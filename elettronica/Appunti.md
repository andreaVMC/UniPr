## Sistemi elettronici
un sistema elettronico è qualcosa che ha degli ingressi (input) e ha delle uscite (output) -> le entrate e le uscite sono sottoforma di segnali elettrici.
![[Pasted image 20240923092222.png]]
==i sistemi elettronici vengono classificati in base alla loro funzione applicativa==.

==Il sensore converte una grandezza fisica in un segnale elettrico==, quindi adatto alla lavorazione da parte del sistema elettronico -> ==un sistema elettronico prende in entrata e da in usciti solo segnali elettrici==.
I ==**sensori**== trasformano grandezze fisiche in segnali elttrici, mentre gli **==attuatori==** trasformano segnali elettrici in grandezze fisiche.
- Sensori = input
- Attuatori = output

## Segnali

==Il segnale è una grandezza che varia nel tempo==, dove ==l'Andamento== (forma d'onda) ==è il modo con il quale un circuito genera e comunica informazioni==
- **segnali digitali** : può assumere numero discreto (finito) di valori
- **segnali analogici** : può assumere un numero infinito di valori 

 ==l'alfabeto è l'insieme di valori assumibili dal segnale== che viene rappresentato.

Si usano i segnali digitali per una questione di rumore della trasmissione, con un segnale digitale è possibile la rigenerazione del segnale in maniera accurata e precisa.
--- start-multi-column: ID_1m3h
```column-settings
Number of Columns: 2
Largest Column: standard
```
## Segnale analogico

![[Pasted image 20240923100106.png]]

--- column-break ---

## Segnale digitale

![[Pasted image 20240923100148.png]]

--- end-multi-column
Come vediamo il segnale digitale dopo esser stato processato è privo di rumore, mentre il segnale analogico non è ripulibile.

## Calcolatori elettronici
==La caratteristica principale dei calcolatori elettronici è la **generalità**, ed è uno strumento che segue un insieme di azione elementari su dei dati per produrre dei risultati==, ma lavora su grandezze e dati digitali.
Quindi noi dovremo ==convertire segnali Analogici in Digitali attraverso una serie di passaggi== che sono:
- **campionamento**: che divide il segnale in campioni temporali
- **quantizzazione**: assegna i valori al segnale analogico attraverso intervalli di valore
- **codifica**: prende i valori dei vari frammenti temporali e crea il segnale digitale finale

![[Pasted image 20240923101815.png]]

------------

## Distanza di Hamming
==La distanza di hamming è il numero di bit diversi che hanno due codifiche di numeri==, per esempio avendo 1 e 2 in binario su una codifica di 5 bit avremo che la distanza di hamming sarà di 2 in quanto:
$$1_{10}=00001_{2}$$
$$2_{10}=00010_{2}$$
qua vediamo che sia il primo che il secondo bit sono diversi, quindi 2 bit diversi, quindi la distanza di hamming è 2. ==Viene utilizzata per sistemare errori di trasmissione.==

## Codice di Gray
deve essre rispettata la regola che due elementi consecutivi che hanno una codifica con distanza di hamming pari ad 1; quindi non avremo più l'ordine:


$$\begin{cases} \\
0001\\
0010 \\
0011 \\
0100 \\
0101 \\
0110 \\
0111 \\
1000 \\
\dots
\end{cases}$$
ma avremo l'ordine:
$$\begin{cases} \\
0001\\
0011 \\
0010 \\
0110 \\
0111 \\
0101 \\
0100 \\
1100 \\
\dots
\end{cases} \\
$$