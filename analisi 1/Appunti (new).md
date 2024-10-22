## Successioni
### Nozione di intorno
L'intorno di un punto $x_{0} \in \mathbb{R}$  è un qualsiasi intervallo $]H,K[$ che contiene $x_{0}$, tale che $H< x_{0}< K$; l'insieme degl'intorni di $x_{0}$ viene denotata con il simbolo $\mathbb{I}_{x_{0}}$; il concetto di intorno va cosi a formalizzare l'idea di "vicino ad n".
Ora si possono anche definire le nozioni di intorno destro e sinistro:
- si dice intorno sinistro di $x_{0}$ qualunque numero $h \in \mathbb{R}:h<x_{0}$
- si dice intorno destro di $x_{0}$ qualunque numero $k \in \mathbb{R}\mathbf{k}>x_{0}$

![[Pasted image 20241019160728.png]]
##### Proprietà degl'intorni
- punti distinti hanno intorni distinti: $\forall x_{0},x_{1} \in \overline{R}, \exists V_{0 } \in I_{0}, V_{1}\in I_{1}:V_{0} \cap V_{1}= \varnothing$
- fissato $x_{0}, \text{se }V_{0} \in I_{0},V_{1} \in I_{0} \to V_{0} \cap V_{1} \in I_{0}$
- se $x_{0} \in R, I_{\varepsilon}(x_{0})=]x_{0}- \varepsilon,x_{0}+\varepsilon[$  e $I_{x_{0}},V\varepsilon>0$ allora vuol dire che intorno ad $x_{0}$ ci sono intervalli di raggio $\varepsilon$ ![[Pasted image 20241019172911.png]]

### Successioni
Si dice successione una qualsiasi funzione $f$ definita su una semiretta $S:=\{n\in N \mid n\geq n_{0}\}, n_{0} \in N$ ;
se il suo codominio è un insieme $A$ si parla di successione di elementi di $A$; per una successione $f:S\to A$ si usa la notazione $\{a_{n}\}_{n}$ dove $a_{n} \in A$ viene ricavata dalla funzione $n\to f(n)=a$

##### proprietà di monotonia
Una successione si può definire monotona se i valori presenti in essa seguono sempre la stessa direzione crescente o decrescente; quindi avendo la successione $\{a_{n}\}_{n}$ è crescente per ogni $n,m \in N:n<m \implies a_{n}\leq a_{m}$; di conseguenza una successione di numeri reali risulta:
- crescente se $\forall n,a_{n}\leq a_{n+1}$
- strettamente crescente se $\forall n,a_{n}<a_{n+1}$
- decrescente se $\forall n,a_{n}\geq<_{n+1}$ 
- strettamente decrescente se $\forall n,a_{n}>a_{n+1}$
### Estremi di successioni
Riscrivendo la nozione di estremi di funzioni per le successioni, deduciamo che l'estremo superiore e inferiore di una successione {$sup_{n}a_{n} \text{ e } inf_{n}a_{n}$} sono i due estremi dell'insieme $a_{n} \mid n \in S$, lo stesso vale per il $max_{n}a_{n}$ ed il $min_{n}a_{n}$; di conseguenza possiamo dividere le successioni in:
1. limitate
	- superiormente: $\exists M \in R:a_{n}\leq M$, ciò vuol dire che $\forall n,an\leq sup_{n}a_{n} \text{ e }\forall \xi >0, \exists \overline{n}:a_{\overline{n}}>sup_{n}a_{n}-\xi$
	- inferiormente:  $\exists M \in R:a_{n}\geq M$, ciò vuol dire che $\forall n,an\geq inf_{n}a_{n} \text{ e }\forall \xi >0, \exists \overline{n}:a_{\overline{n}}<inf_{n}a_{n}-\xi$
	- sia superiormente che inferiormente: $\exists\tilde{M} \in R : \forall n,\mid a_{\overline{n}}\mid\leq\tilde{M}$
2. non limitata
	- superiormente: $\forall M \in R, \exists\overline{n}:a_{\overline{n}}>M$ da cui ricaviamo che $sup_{n}a_{n}=+\infty$
	- inferiormente: $\forall m \in R, \exists\overline{n}:a_{\overline{n}}<m$ da cui ricaviamo che $inf_{n}a_{n}=-\infty$

### Limite di successioni
una successione ha limite $l \in \overline{R}$ per $a_{n}$ che tende ad $l$, se risulta:$$\forall V \in I_{l}, \exists \overline{n}\in N: \forall n\geq\overline{n},a_{n} \in V$$ in altre parole: a partire da un certo punto $\overline{n}$, tutti i termini successivi della successione si trovano dentro un qualsiasi intorno del limite, cioè sono sempre più vicini al valore di limite man mano che la successione progredisce.
Per esempio avendo la successione $a_{n}=2^n$ vediamo come man mano che la $n$ cresce i valori della successione tendono a $+\infty$:
![[Pasted image 20241019174236.png]]
