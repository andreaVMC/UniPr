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
![[assimo elemento separatore]]

$\sqrt{ 2 }$ non è razionale quindi non è seperatore, per tanto è nell'insieme A o in B, sistenendo:
$\sqrt{ 2 } \in \mathbb{R}$ e che esiste un $c \in \mathbb{Q}^{+} : c^2<2$ allora:$$\exists n \in \mathbb{N}^+:\left( c+ \frac{1}{n} \right)^2<2$$
ciò vuol dire che c è un razionale positivo, il quale il quadrato è minore di 2, ma aggiungendo a c un infinitesimo e ne facciamo il quadrato, avremo sempre un numero <2 ma più vicino, quindi non esiste un numero separatore razionale.

### Maggioranti
Un insieme A si dice limitato superiormente se ammette maggioranti M, quindi ogni a appartenente ad A, deve essere minore di ogni elemento dell'insieme dei maggioranti:
$$\forall a \in \mathbb{A}, a\leq M$$
l'insieme dei maggioranti di A si indica con il simbolo: $\mathbb{M}_{\mathbb{A}}$.
per esempio l'insieme $\mathbb{N}$ non è limitato superiormente quindi non ammette maggioranti.
#### L'esistenza del massimo
Oltre a ciò dobbiamo tenere inconsiderazione la possibile esistenza di un massimo dell'insieme A, mettendo caso che $\mathbb{A}=(-\infty,1]$ , ovvero l'insieme A comprende tutti i numeri da meno infinito ad 1 compreso, sappiamo perfettamente che il massimo di questo insieme sarà 1; ma mettendo il caso che $\mathbb{A}=(- \infty,1[$  allora il massimo dell'insieme A sarà un numero infinitamente vicino ad 1 ma pur sempre <1, e per l'assioma del numero separatore sappiamo che esisterà sempre un numero più vicino di un altro ad 1 ma comunque <1; quindi in questo caso l'insieme A non ha massimo.

> nota bene: il massimo dell' insieme:$max(\mathbb{A})$ è uguale al minimo dell'insieme dei maggioranti dell'insieme di A: $min(\mathbb{M_{\mathbb{A}}})$ ; quindi $max(\mathbb{A})= min(\mathbb{M_{\mathbb{A}}})$

### Minoranti
stessa roba dei maggioranti vale per i minoranti, ovviamente qua parliamo di limiti inferiori e si tratta di seguire la regola: $$\forall a \in A , a\geq m$$
#### l'esistenza del minimo 
allo stesso modo , se abbiamo un insieme $A =]-1,+\infty)$ avremo che l'insieme A non ha un minimo in quanto per l'assioma di dedekin 

> nota bene: il minimo dell' insieme:$min(\mathbb{A})$ è uguale al massimo dell'insieme dei minoranti dell'insieme di A: $max(\mathbb{m_{\mathbb{A}}})$ ; quindi $min(\mathbb{A})= max(\mathbb{m_{\mathbb{A}}})$

## Insieme dei numeri immaginari e complessi
L'insieme dei numeri immaginari serve a dare soluzione a quelle operazioni che di fatto non hanno soluzione; l'intero insieme è basato sull' equazione $x^{2} +1 =0$ che vorrebbe a dire $x = \sqrt{ -1 }$ che è impossibile negl'insiemi $\mathbb{R}$ ed $\mathbb{N}$ ,quindi si attribuisce ad una variabile immaginaria $i$ il valore di $\sqrt{ -1 }$, di conseguenza $$i^2=-1$$
### Numeri complessi
Un numero complesso è un numero composto da un numero reale ed un numero immaginario, quindi si dice che l'insieme dei numeri complessi $\mathbb(C)$ è composto nella seguente maniera:
$$\mathbb{C}=\{a+bi:a,b \in \mathbb{R}\}$$
quindi vi è un inclusione stretta di R in C; il numero complesso viene indicato dalla variabile $z$, che è di conseguenza composta dalla parte reale e dalla parte immaginaria i.

##### Operazioni

 - la somma tra due $z$ avviene sommando separatamente parti reali ed immaginarie: $$(3+4i)+(5-7i)=(3+5)+(4-7)i=8-3i$$
 - la moltiplicazione tra due $z$ avviene come una semplice prodotto di somme che già conosciamo, ricordando però che $i^2=-1$ , di conseguenza: $$(3+4i)*(5-7i)=15-21i+20i-28*i^2=15-21i+20i-(28*-1)=15-i+28=43-i$$
 - **il reciproco** di z, ovvero quello che si solito scriveremmo come $\frac{1}{z}$ viene calcolato in questo caso attraverso la formula: $$\frac{1}{z}=\frac{a}{a^2+b^2}-\frac{b}{a^2+b^2}i$$ per esempio il reciproco di z = 3+4i (ovvero quel numero che moltiplicato per z restituisce 1) lo calcoliamo cosi: $$\frac{1}{3+4i}=\frac{3}{9+16}-\frac{4}{9+16}i=\frac{3-4i}{25}$$ e possiamo verificarlo semplicemente moltiplicandolo per z. (se restituisce 1 è verificato)
 - coniugato di z è quel numero che conserva la parte reale di Z ma ha opposta parte immaginaria, se $$z=3+4i \to\overline{z}=3-4i$$
 - il modulo di Z si fa applicando la radice quadrata alle due parti di Z elevate entrambe alla seconda (valore assoluto), quindi: $\mid z\mid = \sqrt{ Rez^2 +Imx^2}$, per esempio: $$\mid_{3}+4i\mid=\sqrt{ 3^2+4^2 }=\sqrt{ 25 }=5$$
##### propietà
- $\overline{z+w} = \overline{z}+\overline{w}$
-  $\overline{z*w} = \overline{z}*\overline{w}$
- $\overline{\overline{z}}=z$
- $z=-\overline{z} \implies \mathbb{Re}z = 0$
- $\mid z\mid=\mid\overline{z}\mid$
- $\mid z+w\mid\leq\mid z\mid+\mid w\mid$
- $\mid z*w\mid=\mid z\mid*\mid w\mid$
- $z*\overline{z}=\mid z\mid^2$
- $\frac{1}{z}=\frac{\overline{z}}{\mid z\mid^2}$
- $\frac{w}{z}=w*\frac{1}{z}=w* \frac{\overline{z}}{\mid x\mid^2}=\frac{w*\overline{z}}{\mid z\mid^2}$
- $\mid z+w\mid^2\leq(\mid z\mid+\mid w\mid)^2$
### Piano di Gaus
il piano di gaus è un piano cartesiano dove la i viene rappresentata sulla delle ordinate (y); quindi per esempio avendo $z=3+4i$ avremo: 
![[Pasted image 20241013152750.png]]
se sei curioso [[piano di gaus]]

Sempre con il piano di gaus possiamo ottenere la somma geometrica di due numeri complessi $z+w$, completando il parallelogramma come formano i due segmenti complessi e facendone il modulo (il modulo di un numero complesso restituisce la distanza tra quel punto e l'origine del piano): 
![[Pasted image 20241013154605.png]]

### Forma trigonometrica
Chiamiamo argomento di z ( arg(z) ) di un numero complesso z appartenente all'insieme dei numeri complessi (escluso lo 0), la misura in radianti dell'angolo formato tra la semiretta passante per 0 e z ed il semiasse positivo reale.

![[Pasted image 20241013204658.png]]

quindi se la condizione $z\neq 0$ viene rispettata si può constatare che: $$z=\mid z\mid(\cos(arg(z))+i*sen(arg(z)))$$
si chiama forma trigonometrica di un numero la scrittura di esso sotto la forma:
$$z=p(\cos o +i*\cos o)$$
dove $p>0$  e  $o \in \mathbb{R}$ ; in questo caso $p$ è il modulo di $z$ e $o$ ne è l'argomento.

Per passare dalla forma algebrica alla trigonometrica, se abbiamo z diverso da 0, avremo che:
$$p=\mid z\mid=\sqrt{ a^2+b^2 }$$
e calcoleremo coseno e seno con la seguente formula:
$$\begin{cases}
\cos o = \frac{\mathbb{R}_{z}}{\mid z\mid}=\frac{a}{\sqrt{ a^2+b^2 }} \\
\sin o = \frac{\mathbb{I}_{z}}{\mid z\mid}=\frac{b}{\sqrt{ a^2+b^2 }}
\end{cases}$$
ovviamente l'argomento di z deve essere compreso tra 0 e $2\pi$.

>NOTA BENE:
-  $\bar{z} = \rho \left(\cos(-\theta)+i\sin(-\theta) \right)$
- $\frac{1}{z} = \frac{1}{\rho}\left(\cos(-\theta)+i\sin(-\theta) \right)$
- $z^n=\rho^n \left(\cos(n*\theta)+i\sin(n*\theta) \right)$
- se $w^n=z$ allora $R^n=\rho \to R=\rho^\frac{1}{n}$
- $z=\rho(\cos(\theta)+i\sin(\theta))$ , $w=R(\cos(\phi)+i\sin(\phi))$ allora: $$z*w=(\rho *R)(\cos(\theta+\phi)+i\sin(\theta+\phi))$$
- allo stesso modo avendo $\frac{z}{w}$ avremo: $$z*w=\frac{\rho}{R}(\cos(\theta-\phi)+i\sin(\theta-\phi))$$
Moltiplicare due numeri complessi, come $w$ e $z$, comporta una rotazione e un cambiamento di dimensione sul piano complesso. Se $w$ ha modulo 1, il prodotto $wz$ risulta in una rotazione di $z$ attorno all'origine di un angolo pari a $\arg(w)$. Ad esempio, moltiplicare $z$ per $i$ lo ruota di un quarto di giro in senso antiorario. Se $w$ ha un modulo diverso da 1, oltre alla rotazione, $z$ viene anche dilatato o compresso in base al modulo di $w$.

#### Radici N-esime di un numero complesso
le radici n-esime di un numero complesso si ottengono "sparpagliando" $n$ numeri complessi lungo una circonferenza, tutti con lo stesso modulo, ma con angoli differenti che si trovano aggiungendo multipli di $2π/n$.

esempio:
![[Pasted image 20241014230921.png]]

### Teorema fondamentale dell'algebra
Il **Teorema Fondamentale dell'Algebra** afferma che ogni polinomio di grado $n$ con coefficienti complessi ha esattamente $n$ soluzioni (dette radici) nei numeri complessi, tenendo conto delle loro molteplicità. Questo significa che se hai un polinomio del tipo $Pn(z)$, dove $z$ è un numero complesso e il grado del polinomio è $n$, ci saranno $n$ soluzioni complesse per l'equazione $Pn(z)=0$.

Ora, se il polinomio ha **coefficienti reali** (anziché complessi), succede una cosa interessante. Se una radice del polinomio è un numero complesso non reale (cioè appartiene ai numeri complessi, ma non ai numeri reali), allora anche il **coniugato** di quel numero complesso sarà una radice del polinomio.
Questo accade perché i polinomi a coefficienti reali hanno una proprietà simmetrica rispetto ai numeri complessi: se una radice è complessa, anche il suo coniugato deve esserlo, con la stessa molteplicità.

### Principio del minimo intero
il principio del minimo intero esprime il buon ordinamento dei numeri naturali.
Applicando il teorema di esistenza dell'estremo superiore si dimostra che ogni insieme $\mathbb{A} \subseteq \mathbb{N}$ (ovvero A sottoinsieme di N) che è non vuoto ha un minimo.

### Principio di induzione
Il principio di induzione serve a dare senso alle definizioni ricorsive, ed è utile nella verifica di propietà che dipendono da un numero naturale.
Se abbiamo un insieme $\mathbb{S} \subseteq \mathbb{N}$ che verifica:
- $0 \in \mathbb{S}$
- $\forall n \in \mathbb{S}\implies n+1 \in \mathbb{S}$
allora $\mathbb{S}=\mathbb{N}$

esempio:
mettendo che volessimo definire il fattoriale (!), sappiamo che la funzione $f:\mathbb{N}\to \mathbb{N}$ e data da:
$$\begin{cases}
f(0)=1 \\
f(n+1)=(n+1)*f(n) \text{ se } n\geq o
\end{cases}$$
quindi come possiamo vedere verificando la funzione $f(n_{0})$ e la funzione di $f(n)$, possiamo verificare la funzione di $f(n+1)$ semplicemente paragonandola alla funzione $f(n)$ già verificata:
$$f(n)=1*2*3*4*\dots*n$$
$$f(n+1) \text{ non verificata, ma } f(n)*(n+1) \text{ è verifcata }$$
$$\text{di conseguenza anche } f(n+1) \text{ viene verificata} $$
#### Principio di induzione applicato ai predicati
Il principio di induzione applicato ai predicati viene utilizzato per dimostrare la verità di una proposizione $P(n)$, definita su numeri naturali, per ogni $n∈ \mathbb{N}$. Vediamo di spiegare come viene applicato.

Il principio di induzione dice che, se si hanno le seguenti due proprietà per un predicato $P(n)$:

1. **Base**: $P(0)$ è vero (ossia la proposizione è vera per il caso base, solitamente $n=0$).
2. **Passo induttivo**: per ogni $n \in \mathbb{N}$, se $P(n)$ è vero, allora risulta vero anche $P(n+1)$.

Se queste due proprietà sono soddisfatte, possiamo concludere che $P(n)$ è vero per ogni $n \in \mathbb{N}$. Questo procedimento funziona perché la base $P(0)$ fornisce il punto di partenza, e il passo induttivo ci permette di estendere la verità del predicato a tutti i numeri naturali.

##### Ricaviamo il principio di induzione dal principio del minimo intero
- **principio del minimo intero**: ogni sottoinsieme non vuoto dei numeri naturali ha un elemento minimo.
- Vogliamo dimostrare che un proposizione $P(n)$ è vera per un valore iniziale $n_{0}$, e se per ogni $n \in \mathbb(N)$ la verità $P(n)$ implica la verità $P(n+1)$, allora $P(n)$ è vera per tutti i numeri naturali.
- Supponiamo per assurdo che esista un valore $n$ per cui $P(n)$ non è vero, e prendiamo in considerazione l'insieme $S=\{n \in N | P(n) \text{ è falso}\}$, di conseguenza sappiamo che $S$ non è vuoto perché vi è almeno un elemento $n$.
- Utilizzando il principio del minimo intero su $S$ (insieme non vuoto di $N$), sappiamo che esiste un numero minimo $m \in S$ tale che $P(m)$ è falso, ma per ogni $k<m, P(k)$ è vero.
- Sapendo che $P(n_{0})$, dove $n_{0}$ è il valore iniziale, è verificato, e quindi non può essere $m=n_{0}$ ,di conseguenza $m>n_{0}$
- ora che sappiamo che $P(m-1)$ è vero, in quanto $m$ è il valore minimo per cui $P(m)$ risulta falso. Ma dall'ipotesi del principio di induzione, se $P(m-1)$ è verificato, allora anche $P(m-1+1)=P(m)$ dovrebbe esserlo; ciò va cosi a contraddire la scelta di $m$ come elemento minimo di $S$
- Quindi la nostra assunzione iniziale, ovvero che esiste un numero minimo $m$ tale che $P(m)$ sia falso, porta ad una contraddizione; portandoci cosi a concludere che $S$ sia un insieme vuoto, e che quindi non esistono numeri naturali $n$ per cui $P(n)$ sia falso; di conseguenza $P(n)$ è verificato per tutti i naturali.
In conclusione riusciamo a derivare il principio di induzione dal principio del minimo intero per assurdo; ovvero che se una proprietà $P$ fosse falsa per un qualunque numero naturale $n$, esisterebbe un numero naturale minimo per cui la proprietà è falsa, ma ciò porterebbe ad una contraddizione con l'ipotesi del passo induttivo. Di conseguenza la proprietà deve essere verificata per tutti i naturali.
