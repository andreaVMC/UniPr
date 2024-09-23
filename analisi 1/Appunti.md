## Funzione

Una funzione $f$ è una relazione tra gli insieme di $A$ e $B$, che sono rispettivamente dominio e codominio, tale che la legge $f$ verifica che: 

> per ogni $a$ appartenente all'insieme $A$, esiste una sola $b$ appartenente all'insieme $B$ tale che $b=f(a)$
$$\forall a\in A,\exists ! b \in B : f(a)=b $$
----------

## L'immagine
La funzione immagine prende un sottoinsieme di $A$ e ne restituisce il sottoinsieme corrispondente di $B$, quindi l'insieme delle parti di $A$ fa riferimento all'insieme delle parti di $B$ ( $f:P(A)\to P(B)$ )  e viene definita in questa maniera:
$$f(E):={f(a)|a \in E}$$
dove $E$ è un qualsiasi sottinsieme di A, ed $f(E)$ è il sottinsieme di $B$ che contiene tutte le immagini degl'elementi di $E$.
### L'insieme immagine
Se prendiamo tutto l'insieme di $A$ e lo mettiamo in $E$ (invece che solo un sottoinsieme), l'immagine di $A$ sotto la funzione $f$ prende il nome di immagine di $f$:
$$im f:=f(A)$$
questo forma il sottoinsieme di B formato da tutte le immagini degl'elementi A
quindi l'insieme immagine si trova all'interno del Coodominio

## Controimmagine
La funzione controimmagine, al contrario della funzione immagine va a restituire gli elementi dell'insieme $A$ associati all'elemento dell'insieme $B$ sul quale viene applicata la funzione immagine, quindi l'insieme delle parti di $B$ fa riferimento all'insieme delle parti di $A$  ( $f:P(B)\to P(A)$ ), e si definisce:
$$f^{-1}(F):={a \in A | f(a \in F)}$$
### L'insieme controimmagine
quindi l'insieme delle controimmagini presenti nel dominio formano l'insieme controimmagine

spiegazione grafica:
![[immagine & contro]]

----------
## Grafico

Il grafico di una funzione $G(f)$ è il sottoinsieme del prodotto cartesiano tra il dominio ed il codominio $AXB$ (ovvero tutte le coppie possibili tra $A$ e $B$) e viene definito cosi:

> il $G(f)$ è uguale all'insieme di coppie $a$ e $b$ ristretto alle $a$ appartenenti ad $A$, ed alle $b$ appartenenti a $B$, dove $f(a)=b$

$$
G(f) = {(a,b)|a \in A, b \in B, f(a)=b}
$$
--------------------
## Iniettiva
Una funzione si dice iniettiva quando nessuna delle ordinate si incorcia con più di un punto della funzione.

>  Quindi $f:A\to B$ si dice iniettiva se per ogni $a1,a2$ appartenente all' insieme $A$, $a_{1}$ è diverso da $a_{2}$ come $f(a_{1})$ è diverso da $f(a_{2})$ 

$$\forall a_{1},a_{2}\in A,[a_{1}\ne a_{2} \to f(a_{1}) \ne f(a_{2})]$$
--- start-multi-column: ID_a1dg
```column-settings
Number of Columns: 2
Largest Column: standard
```

### Iniettiva
![[Pasted image 20240923162927.png]]


--- column-break ---

### non iniettiva
![[Pasted image 20240923162825.png]]

--- end-multi-column

------------------
## Suriettiva
Una funzione si dice suriettiva quando l'immagine della funzione corrisponde al codominio $B$; quindi per ogni valore y del codominio vi è un valore x corrispondente della funzione.

![[Pasted image 20240923164129.png]]

> quindi $f:A\to B$ si dice suriettiva se per ogni $b$ appartenente a $B$, esiste almeno un' $a$ appartenente ad $A$ tale che $f(a) = b$
$$\forall {b}\in B, \exists a \in A : f(a)=b$$
-----------
## Biettiva / Biunivoca
Una funzione si dice biettiva o biunivoca se è sia iniettiva che suriettiva

>per ogni y presente nel codominio (uguale all'immagine della funzione), è presente una sola x corrispondente tale che f(x) = y
$$
\forall b \in B, \exists!a \in A:f(a)=b
$$

se la funzione è biunivoca possiamo ricavarne l'inversa $f^{-1}(b)=a$ rappresentando la funzione inversa: $$f^{-1}:B\to A, f^{-1}(b)=a \implies f(a)=b$$