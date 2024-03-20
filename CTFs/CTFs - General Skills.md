
Shell commands:
➢ cd dir: naviga nella cartella dir; . è la cartella corrente, .. è la cartella superiore 
➢ ls dir: lista i file nella cartella dir; senza argomenti lista i file della cartella corrente 
➢ mkdir dir: crea la cartella dir 
➢ cat f1: stampa il contenuto del file f1 
➢ cp f1 f2: copia il file f1 nel file f2 ➢ mv f1 f2: sposta il file f1 nel file f2 
➢ rm f1: rimuove il file f1 (attenzione: non viene spostato in un cestino) 
➢ file f1: fornisce informazioni sul tipo del file f1 
➢ head f1 –n N: stampa le prime N righe del file f1 
➢ tail f1 –n N: stampa le ultime N righe del file f1 
➢ more f1: mostra il contenuto del file f1 riga per riga (l’altezza è limitata a quella del terminale) 
➢ strings f1 –n N: stampa le stringhe leggibili di lunghezza almeno N contenute nel file f1 
➢ grep patt f1: cerca il pattern patt nel file f1
➢ ssh user@host: crea una connessione al server host, fornendo un terminale come utente user 
➢ nc host port: crea una connessione TCP al server host sulla porta port 
➢ In caso di dubbi... 
	➢ man cmd: manuale del comando cmd 
	➢ Google


# https://overthewire.org/wargames/bandit/bandit0.html

## Lv. 0:

per collegarsi ad un sito si usa `ssh` 

```
matti@kraxt:~$ ssh bandit0@bandit.labs.overthewire.org -p 2220
```

prima del sito metto il nome utente con cui colelgarmi, bandit0. Letteralmente sarebbe: << Collegami come "bandit0" a (@)  bandit.labs.overthewire.org nella porta 2220. 
Dopo verrá chiesta la password, anch'essa bandit0. E siamo dentro!

## Lv. 0->1:

una volta dentro troveremo un file readme nella home. Lo apriamo e al suo interno c'é la password per connettersi come bandit1.
Loggiamo fuori da bandit0
```
bandit0@bandit:~$ logout
```
Connettiamoci come bandit1:
```
matti@kraxt:~$ ssh bandit1@bandit.labs.overthewire.org -p 2220
```
e inseriamo la password trovata prima.
🖥 Eccoci loggati come bandit1.

## Lv. 1->2

Ottenere questa password sembra facile ma é un pochetto _tricky_. 
Per visualizzare il contenuto di un file nominato "-" non possiamo usare `cat`e basta.

Ecco come fare:

```
bandit1@bandit:~$ ls
	-
bandit1@bandit:~$ cat ./-
	rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
```

Ecco ottenuta la password :)

Sloggiamoci:

`bandit1@bandit:~$ logout`

E colleghiamoci al livello 3:

`matti@kraxt:~$ ssh bandit2@bandit.labs.overthewire.org -p 2220`

## Lv. 2->3

Questo é abbastanza facile.
Se ci sono degli spazi nel nome del file basta racchiuderlo in un paio di "" e usare `cat` come sempre, ed ecco la nostra password .

```
bandit2@bandit:~$ ls
	spaces in this filename
bandit2@bandit:~$ cat "spaces in this filename"
	aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
```

Come sempre logout e connessione al nuovo livello. (da ora in poi questo passaggio é sottointeso dopo aver trovato la password)


## Lv. 3->4

Il file contenente la  password si trova nella cartella "inhere".
Peró il file é nascosto. Per verificare che sia realmente qui usiamo `du -h` che ci fará vedere che qualcosa di 8Kb é all'interno della cartella quindi ecco il nostro file. Ma come vediamo il suo contenuto?
Usiamo `find`
Ecco cosa otteniamo:

```
bandit3@bandit:~$ ls
	inhere
bandit3@bandit:~$ cd inhere
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ du -h
	8.0K	.
bandit3@bandit:~/inhere$ find 
	.
	./.hidden

```

Adesso possiamo usare `cat`

```
bandit3@bandit:~/inhere$ cat ./.hidden
	2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
```


## Lv. 4->5

Sta volta dobbiamo capire quali tra questi file é in un carattere da noi leggibile. Il probelma dice che sono uno dei 10 lo é. Per capire il tipo di file possiamo usare `file ./*` con questo comando indichiamo tutti (`*`) i file all'interno della cartella corrente (`.`) 

```
bandit4@bandit:~$ ls
	inhere
bandit4@bandit:~$ cd inhere
bandit4@bandit:~/inhere$ file ./*
	./-file00: data
	./-file01: data
	./-file02: data
	./-file03: data
	./-file04: data
	./-file05: data
	./-file06: data
	./-file07: ASCII text
	./-file08: data
	./-file09: data
bandit4@bandit:~/inhere$ cat ./-file07
	lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
```


## Lv. 5->6

Dobbiamo trovare un file con delle determinate proprietá che sono:
	- human-readable
	- 1033 bytes in size
	- not executable

Per fare ció entriamo nella cartella e qui usiamo il comando `find`ma con degli attributi, `-type f` indica che vogliamo sono file, `-size 1033c` indica il peso del file.

```
bandit5@bandit:~$ ls
	inhere
bandit5@bandit:~$ cd inhere
andit5@bandit:~/inhere$ find . -type f -size 1033c
	./maybehere07/.file2
bandit5@bandit:~/inhere$ cd ./maybehere07
bandit5@bandit:~/inhere/maybehere07$ cat .file2
	P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
```

Easy peasy. No?

## Lv 6->7

Questo livello é abbastanza complicato. Dobbiamo trovare la password ma é conservata dall'utente bandit7 che fa parte del gruppo bandit6, il file é grande 33 bytes

Per farlo usiamo find con degli attributi: 

```
bandit6@bandit:~$ find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
	/var/lib/dpkg/info/bandit7.password

```

Bene, ora al prossimo  livello O_o

## Lv. 7->8

Questa sembra facile no? Circa.

Se  proviamo a visualizzare il contenuto del file data.txt vediamo che si sono un pó di password ;)

Per trovare la password che sta vicino alla parola "millionth" possiamo usare `grep`

```

bandit7@bandit:~$ ls
	data.txt
bandit7@bandit:~$ grep "millionth" data.txt
	millionth	TESKZC0XvTetK0S9xNwm25STk5iWrBvP

```

Easy!


## Lv. 8->9


Questo é complicato, o lo é stato per me.
Dobbiamo trovare la password in un file, data.txt, questa é l'unica che si ripete una sola volta.
Per farlo combiniamo `sort` e `uniq`, ecco come:

```
bandit8@bandit:~$ ls
	data.txt
bandit8@bandit:~$ sort data.txt | uniq -u
	EN632PlfYiZbn3PhVK3XOGSlNInNE00t
```


## Lv. 9->10

Questo era easy.

Dobbiamo cercare nel file, quella riga leggibile dall'uomo che contiene la password ed é preceduta da un pó di "=", peró ci sono anche righe leggibili ma errate.

Per trovarla basta usare `strings`
```
bandit9@bandit:~$ strings data.txt
	========== G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
```

La password non é il solo output, ma é l'unica riconducibile ad una password.