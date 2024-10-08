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
### Iniettiva
![[Pasted image 20240923162927.png]]
### non iniettiva
![[Pasted image 20240923162825.png]]

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

------------

## Funzioni composte
Un funzione composta sostanzialmente è la composizione, indicata dal simbolo $\circ$, per esempio avendo le due funzioni: 
- $A\to f(a) \to B$ dove la funzione $f$, passa dall'insieme $A$ all'insieme $B$
- $B \to g(b) \to C$ dove la funzione $g$, passa dall'insieme $B$ all'insieme $C$
possiamo creare una funzione composta $g \circ f$, che implicherà un passaggio dall'insieme A all'insieme C:
$$g\circ f:A\to G \implies (g \circ f)(a)=g(f(a))$$
### Proprietà
- se sia $f$ che $g$ sono iniettive, allora anche la loro composizione $g \circ f$ sarà iniettiva:$$\forall a_{1},a_{2} \in A, a_{1} \ne a_{2} \implies f(a_{1})\ne f(a_{2}),g(a_{1})\ne g(a_{2}) \implies(g \circ f)(a_{1})\ne(g \circ f)(a_{2})$$
- se sia $f$ che $g$ sono suriettive, allora anche la loro composizione $g \circ f$ sarà suriettiva:$$\forall c \in C, \exists a \in A: (g \circ f)(a)=c$$
- se sia $f$ che $g$ sono biunivoche, allora anche la loro composizione $g \circ f$ sarà biunivoca

### Composizione inversa
allo stesso modo della composizione $g \circ f$ che ci fa passare dall'insieme $A$ all'insieme $C$, esistono le composizioni inverse che ci fanno ritornare all'insieme di partenza:
$$(g \circ f)^{-1} = f^{-1} \circ g^{-1}$$
----------------
## Funzioni reali monotone
Una funzione monotona è una funzione con andamento, crescente o decrescente, che non cambia mai; in una funzione monotona crescente infatti non può esserci nemmeno un punto in cui la funzione decresca e viceversa, in sostanza le due leggi per una funzione monotona sono:

- crescente: $\forall x_{1},x_{2} \in A,x_{1}<x_{2}\implies x_{1}<x_{2}$
- decrescente:$\forall x_{1},x_{2} \in A,x_{1}<x_{2}\implies x_{1}>x_{2}$

bisogna anche fare una distinzione tra funzioni monotone strettamente cresc/decresc, e funzioni monotone debolmente cresc/ decresc:

- le funzioni strettamente monotone non hanno segmenti della funzione in cui la loro variazione può essere pari a 0, e quindi $x_{1}$ sarà sempre o maggiore o minore di $x_{2}$ ; la legge in particolare di queste è $$\forall x_{1},x_{2} \in A,x_{1}<x_{2}\implies x_{1}<x_{2}$$ $$\forall x_{1},x_{2} \in A,x_{1}<x_{2}\implies x_{1}>x_{2}$$
- le funzioni debolmente monotone invece hanno punti della funzione in cui rimangono invariate e quindi è possibile la condizione $x_{1}=x_{2}$ ; di conseguenza le leggi saranno:$$\forall x_{1},x_{2} \in A,x_{1}<x_{2}\implies x_{1}\leq x_{2}$$ $$\forall x_{1},x_{2} \in A,x_{1}<x_{2}\implies x_{1}\geq x_{2}$$
### caso particolare
ovviamente una funzione come detto prima non può essere sia strettamente crescente che strettamente decrescente, ma al contrario può essere debolmente crescente e debolmente decrescente contemporaneamente; ciò accade quando una funzione non subisce alcuna variazione (costanti) rispettando entrambe le leggi delle funzioni debolmente monotone, come per esempio:
![[Pasted image 20240924220036.png]]
### strettamente monotone & iniettivita
una funzione strettamente monotona, quindi strettamente crescente o decrescente sarà sempre iniettiva; in quanto ne rispetta la legge; al contrario, non tutte le funzioni iniettive sono strettamente monotone, per esempio: 
![[Pasted image 20240924220435.png]]
la funzione è iniettiva in quanto nessuna $y$ incontra più di una $x$ della funzione, ma allo stesso tempo non è strettamente monotona in quanto non mantiene un andamento crescente o decrescente, bensì si alterna.

-----------
## Funzioni simmetriche
le funzioni simmetriche sono coloro che si specchiano sul grafico e si dividono in due gruppi:
- **pari**: ovvero quelle che si specchiano sull'asse delle ordinate
![[Pasted image 20240924221028.png]]
![[Pasted image 20240924221225.png]]

nelle funzioni pari in particolare vediamo come sia ad $x$ che al suo opposto corrisponde la stessa y, quindi possiamo ricavarne la legge: $$\forall x\in A, f(x)=f(-x)$$
- **dispari**: ovvero quelle che si specchiano sull'origine

![[Pasted image 20240924221438.png]]

![[Pasted image 20240924221555.png]]

qua vediamo come ad $x$ corrisponda una $y$ che è esattamente l'opposto della $y$ che corrisponde all'opposto di $x$, quindi possiamo ricavarne la legge:
$$\forall x\in A,f(-x)=-f(x)$$
### cos & sin
di conseguenza seguendo questi ultimi ragionamenti e leggi troveremo come i, coseno è pari, mentre il seno è dispari:
#### cos(x)
![[Pasted image 20240924222053.png]]
#### sin(x)
![[Pasted image 20240924222153.png]]


-------------

## Funzioni valore assoluto
La funzione valore assoluto $f$ restituisce il valore massimo tra la $a$ fornita alla funzione ed il suo opposto, quindi: $f(a) = max(a,-a) \to \mid a\mid$ ; di conseguenza avremo che la funzione si comporta nella seguente maniera: 
$$\mid a\mid = \begin{cases}  a \to a\geq 0 \\ \\
-a \to a\leq 0
\end{cases}$$
il grafico di tale funzione quindi sarà rappresentato solo nella parte positiva del grafico, dove la parte negativa verrà specchiata sull'asse delle ordinate, quindi prendendo in considerazione $\mid x \mid$ :
![[Pasted image 20240925110130 1.png]]

### Propietà
- $\mid a\mid=0 \to a=0$
- $-\mid a\mid\leq a\leq\mid a\mid$
- $\mid-a\mid=\mid a\mid$
- se $\mid a\mid \leq b$  allora $-b \leq a \leq b$ , con $b$ che necessariamente de essere $b\geq0$ ![[Pasted image 20240925111519 1.png]]
 
### disuguaglianze triangolari
#### prima
>la prima disuguaglianza triangolare afferma che per ogni $a,b$ appartenenti all'insieme $\mathbb{R}$, il valore assoluto di $a+b$  è minore o uguale al valore assoluto di $a$ più il valore assoluto di $b$:

dimostrazione: 
$$\forall a,b \in \mathbb{R} \mid a+b\mid \leq \mid a\mid+\mid b\mid$$
$$\begin{cases} 
-\mid a\mid\leq a\leq\mid a\mid \\
-\mid b\mid\leq b\leq\mid b\mid
\end{cases}= -(\mid a\mid+\mid b\mid)\leq a+b\leq\mid a\mid+\mid b\mid$$
$$\mid a\mid\leq b \implies -b\leq a\leq b$$
$$A=\mid a+b\mid, B=\mid a\mid+\mid b\mid \to\mid A\mid\leq\mid B\mid
$$
$$A\leq B = \mid a+b\mid\leq\mid a\mid+\mid b\mid$$
### seconda
>la seconda disuguaglianza triangola **di continuità** afferma che il valore assoluto della differenza degl'assoluti di $a$ e $b$, per intenderci:  $\mid(\mid a\mid-\mid b\mid)\mid$ , è minore o uguale alla differenza assoluta tra i due

$$\forall a,b \in \mathbb{R} \mid\mid a\mid-\mid b\mid\mid \leq\mid a-b\mid$$
che andiamo a dimostrare utilizzando la prima disuguaglianza triangolare abbiamo:
$$\mid a\mid=\mid(a-b)+b\mid\leq\mid a-b\mid+\mid b\mid$$
qua andiamo ad utilizzare la prima disuguaglianza triangolare, e tenendo presente $-B\leq A\leq B$ andiamo a verificare entrambi i simboli:
- prima verifichiamo $A\leq B$ con:
$$\mid a\mid-\mid b\mid\leq \mid a-b\mid$$
qua come possiamo vedere $\mid a-b\mid = B,\mid a\mid-\mid b\mid=A$, di conseguenza $A\leq B$

- poi verifichiamo $-B \leq A$ prendendo l'opposto di $\mid a-b\mid$ ovvero $-B$ che è  $-\mid a-b\mid$
   $$-\mid a-b\mid\leq\mid a\mid-\mid b\mid$$
cosi da ottenere appunto $-B\leq A$

Infine otterremo cosi che $-\mid a-b\mid\leq \mid a\mid - \mid b\mid \leq \mid a-b\mid$, ovvero, tenendo presente della nostra notazione: $\mid a-b\mid = B,\mid a\mid-\mid b\mid=A$:
$$-B\leq A\leq B$$
e grazie a questa proprietà della funzione assoluta verifichiamo la seconda disuguaglianza triangolare di continuità.

### ==ricopiare esempi di esercizi==

--------------------

# Insiemi Numerici
una relazione sull' insieme $\mathbb{X}$, che è sottoinsieme dell'insieme $\mathbb{R}$, nel piano cartesiano formato da $\mathbb{X}*\mathbb{X}$, dove troviamo due punti $x,y \in \mathbb{R}$, questi due punti si dicono in relazione
## Relazioni di equivalenza
una relazione di equivalenza è tale se fra i due punti in relazione ($x,y$) vengono rispettate le 3 propietà:
- **riflessiva**: x in relazione con x, che si scrive $\forall x \in \mathbb{X} x \simeq x$
- **simmetrica**: x in relazione con y e viceversa, si scrive $\forall x,y \in \mathbb{X} x\simeq y\implies y\simeq x$
- **transitiva**:  x in relazione con y, y in relazione con z, quindi x in relazione con z, si scrive: $\forall x,y,z \in \mathbb{X} x\simeq y,y\simeq z \implies x\simeq z$

i punti $(x,y)$ e $(x_{0},y_{0})$ sono in relazione tra loro se rispettano il criterio: $x-x_{0}=y-y_{0}$
data questa nozione di equivalenza si dice classe di equivalenza: $[x]={y\in \mathbb{X}: y \simeq x}$
## Relazioni d'ordine
una relazione d'ordine tra due insieme si denota con il simbolo $\leq$ di precedenza, e si dice che un insieme X preceda nell'ordine un altro insieme se sono rispettate le propietà:
- riflessiva
- transitiva
- <font color="#ff0000">anti-simmetrica</font>: ovvero $x\leq y , y\leq x \implies x=y$

### esempio
avendo $\mathbb{U} , \mathbb{X}=P(\mathbb{U})$ dove X è l'insieme della parti di U, abbiamo che $\mathbb{A},\mathbb{B} \in P{\mathbb{U}}$, da qui possiamo constatare che:
- $\mathbb{A}\leq \mathbb{B}$ se ogni elemento di A è elemento anche di B
- $\mathbb{A}\leq \mathbb{B}$ e $\mathbb{B}\leq \mathbb{A}$ se $\mathbb{A}= \mathbb{B}$
- $\mathbb{A}\leq \mathbb{B}$ e $\mathbb{B}\leq \mathbb{A}$ quindi $\implies\mathbb{A}\leq \mathbb{C}$

### Relazione d'ordine totale
una relazione d'ordine si dice totale ==quando gli elementi sono confrontabili==

## Insieme numeri reali
Partendo dalla dichiarazione: $(\mathbb{X} ,+,*,\leq)$ dove il + ed il $*$ vanno ad indicarci la presenza di 4 assiomi per simbolo, mentre il $\leq$ va ad indicarci che la composizione interna dell'insieme è una relazione d'ordine totale.
In totale gli assiomi dell'insieme dei numeri razionali $\mathbb{R}$ è composto da 11 assiomi.

>Assioma: Principio evidente per sé, e che perciò non ha bisogno di esser dimostrato, posto a fondamento di una teoria deduttiva

Per definire l'insieme dei numeri reali $\mathbb{N}$ bisogna definire un ==12° assioma, detto Assioma di Dedekind==, che dice che per ogni $\mathbb{A},\mathbb{B}\subset \mathbb{R}$ tali che $\forall a \in A, b \in B, a\leq b$ allora esiste un elemento $c \in \mathbb{R}$ tale da separare i due insiemi, e quindi: $\forall a \in \mathbb{A}, b \in \mathbb{B} , a\leq c\leq b$, questo viene chiamato anche ==assioma dell'elemento separatore==.

