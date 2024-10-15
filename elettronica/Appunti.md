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
$$----------------

## Minimizzare una rete
Avere una rete che restituisce $y$ ed una che restituisce $y_{min}$, ciò vuol dire minimizzare una rete.

>pagina 65 del libro
### usa teoremi algebra booleana
![[Pasted image 20241008085413.png]]

--------
## Complemento a 2

- **Cos'è:** Una tecnica più avanzata per rappresentare numeri negativi. Invertendo i bit e aggiungendo 1 al risultato, si facilita l'esecuzione di operazioni aritmetiche.
- **Applicazioni:** Utilizzato nei moderni computer per rappresentare numeri negativi e per eseguire operazioni aritmetiche efficientemente, semplificando la progettazione hardware.

- **Rappresentazione:** Un bit è dedicato al segno (0 per positivo, 1 per negativo). Gli altri bit rappresentano il valore assoluto.
- **Esempio:** In una rappresentazione con 8 bit:
    - **+5** = 00000101
    - **-5** = 10000101

### Complemento a 2

- **Metodo:** Consente una rappresentazione più efficiente e facilita le operazioni aritmetiche.
    
- **Passaggi per ottenere il complemento a 2 di un numero binario:**
    
    1. **Inversione dei bit:** Converti 0 in 1 e viceversa.
    2. **Aggiungi 1** al risultato dell'inversione dei bit.
- **Esempio:** Rappresentazione di -5 in 8 bit:
    
    1. **5 in binario:** 00000101
    2. **Inversione dei bit:** 11111010
    3. **Aggiungi 1:** 11111011 (complemento a 2 di -5)
#### ex appunti:
- Complemento ad 1: serve per rappresentare i numeri negativi nei byte, il primo bit diventa un bit di segno che se è a 0 significa che il numero è positivo, mentre se è a 1 significa che il numero è negativo; il complemento ad 1 si calcola convertendo tutti i bit di un byte nell'opposto, per esempio se abbiamo 00011011 diventerà 11100100
- complemento a 2: si utilizza per rappresentare i negativi nel binario, daco che il complemento ad 1 è stato deprecato; si fa utilizzando il complemento ad 1 del byte di un numero assoluto ed aggiungendo 1; per riconvertirlo si controlla se il bit di segno è uguale ad 1 in tal caso si rifa il complemento ad 1 e si aggiunge dinuovo 1


converti numero in binario -> 63=00111111 -> not del numero -> 11000000 -> aggiungo 1 -> 11000001 = -63

per verificare: tolgo 1 e faccio il not del binario.

---------

## Tabella della verità
lega quello che succede alle porte e nel circuito, all'uscita finale

-----
## concetto di indifferenza
Nell'algebra booleana, l'indifferenza (o condizione di don't care) si riferisce a una situazione in cui il valore di una variabile logica non influisce sull'uscita finale della funzione logica. Questi valori possono essere utilizzati per semplificare espressioni logiche, poiché possono essere assegnati a 0 o 1 per ottenere la forma più semplice della funzione.

## Ottimizzazione della rete $\to$ rete ottima
meno ritardo
meno gate
meno ingressi per gate

### Espressione normale
parliamo di espressioni sp o ps

- **Espressione minima**: la forma più semplificata di una funzione booleana, che usa il minor numero possibile di termini e variabili.
- **Rete di costo minimo**: una rete logica che realizza una funzione booleana con il minor numero possibile di porte logiche o connessioni.
- **Implicante primo**: un termine che non può essere ulteriormente semplificato e che copre almeno una combinazione di valori di verità della funzione.
- **Formula duale dell'implicante primo**: si ottiene scambiando AND con OR e viceversa nella forma canonica dell'implicante primo.
- implicato primo: somma di n o meno varibili della funzione in forma vera o negata, dalla quale non è possibile eliminare alcun letterale senza perdere la sua propietà di implicare la fuinzione ovvero di valere 0
- espressione irridondante: qualsiasi espressione dalla quale non è possibilie eliminare termini senza invalidare l'equivalenza con l'espressione di partenza

## Mappa di karnau
![[Pasted image 20241015095538.png]]ogni casella è un mintermine