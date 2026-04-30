# Elementi di Teoria degli Insiemi  

## Numeri Naturali \\( \mathbb{N} \\)
Sia \\( \mathbb{N} \\) = {0, 1, 2, ...} l'insieme dei numeri naturali, diamo - attraverso gli _assiomi di peano_ - 
la definizione formale di tale insieme.

### def
Data la terna \\( (\mathbb{N}, \sigma, 0)  \\), in cui \\( \mathbb{N} \\) è un insieme, \\( \sigma \\colon \mathbb{N} \to \mathbb{N}  \\) è un'applicazione e \\( 0  \in \mathbb{N}\\)  
Valgono le seguenti condizioni:
- \\( \mathbb{N}_1 \\): \\( \sigma \\) è iniettiva.
- \\( \mathbb{N}_2 \\): \\( 0 \notin Im(\sigma) \\)
- \\( \mathbb{N}_3 \\): ogni sottoinsieme \\( U \\) di \\( \mathbb{N} \\) tale che:
  - (a): \\( 0 \in U \\)
  - (b): \\( k \in U \implies \sigma(k) \in U \space \forall k \\)  

  coincide con tutto \\( \mathbb{N} \\)

l'elemento \\( \sigma(n) \\) è detto **successivo** di \\( n \\);  
il postulato \\( \mathbb{N}_3 \\) è detto principio di [_induzione matematica_](https://it.wikipedia.org/wiki/Principio_d%27induzione).
\\( \space\space \square  \\)

## Operazione binaria 
### def 
Un'applicazione \\( S: S \times S \to S \\) è detta **operazione binaria** (anche[^1] _legge di composizione_, nella fattispecie **interna**), ossia una legge che associa ad ogni 
coppia \\( (a, b) \in S \\) un ben determinato elemento di \\( S.  \space\space \square \\)
> **Nota**: si parla di legge di composizione **esterna** nel caso \\( R \times S \to S \mid R \ne S \\) 
>

### esempi 
- Addizione in \\( \mathbb{Z} \\)
\\[
  \\begin{aligned}
  +\colon \mathbb{Z} \times \mathbb{Z} &\to \mathbb{Z} \\\\
  (a, b) &\mapsto a \mathbin{+} b
  \\end{aligned}
\\]  

dove \\( c \overset{\text{def}}{=} a + b \\)  
con \\( a, b, c \in \mathbb{Z} \\)

- Unione tra sottoinsiemi 
\\[
  \\begin{aligned}
  \cup\colon \mathcal{P}(X) &\times \mathcal{P}(X) \to \mathcal{P}(X) \\\\
  (A, B) &\mapsto A \cup B
  \\end{aligned}
\\]  

dove \\( X \\) è un insieme, \\( \mathcal{P}(X) \\) è l'insieme delle parti;  
\\( C \overset{\text{def}}{=} A \cup B \\)  
e vale \\( A, B, C \in \mathcal{P}(X) \\)

## Struttura algebrica 
### def 
Chiamiamo **struttura algebrica** l'oggetto matematico composto da un insieme \\( S \\) che gode di 
una o più _operazioni n-arie_ che soddisfano determinati assiomi. \\( \space\space \square  \\)

## Operazioni definite su \\( \mathbb{N} \\)
Tramite gli assiomi di Peano possiamo definire su \\( \mathbb{N} \\) due operazioni binarie. 

### Somma
#### def
Comunque presi \\( n, m \in \mathbb{N} \\), allora vale
\\[
\begin{aligned}
n \mathbin{+} m \overset{\text{def}}{=} 
\begin{cases} 
\underbrace{\sigma(\sigma(\cdots \sigma}_{m \text{ volte}}(n))) & \text{se } m > 0 \\\\
n & \text{se } m = 0 
\end{cases}
\end{aligned}
\\]  
\\( \space\space \square  \\)  
il numero \\( n \mathbin{+} m \\) è detto _somma_ di \\( n \\) ed \\( m \\).

#### corollario
Dalla definizione di cui sopra segue:  
\\( \sigma(n) = n \mathbin{+} 1 \\) dove l'elemento \\( 1 = \sigma(0) \\).

### Prodotto
#### def 
Comunque presi \\( n, m \in \mathbb{N} \\), allora vale 
\\[
\begin{aligned}
n \cdot m \overset{\text{def}}{=}
\begin{cases}
\underbrace{n + n + \dots + n}_{m \text{ volte}} & \text{se } m > 0 \\\\
0 & \text{se } m = 0
\end{cases}
\end{aligned}
\\]
\\( \space\space \square  \\)  
il numero \\( n \mathbin{\cdot} m \\) è detto _prodotto_ di \\( n \\) ed \\( m \\).

## Principio del buon ordinamento  
### trattazione intuitiva
Ogni sottoinsieme dei numeri naturali non vuoto contiene un elemento che è minore di tutti gli altri, ovvero ammette un elemento **minimo**. Un tale insieme si dice _ben ordinato_. 

> **Nota**: tale definizione è [equivalente](https://it.wikipedia.org/wiki/Principio_del_buon_ordinamento#Equivalenza_con_il_principio_di_induzione) al già citato 
> principio di induzione. 
>

### def 
\\[
  X \subseteq \mathbb{N} \implies \bar{a} \in A \mid \bar{a} \leq a, \forall a \in A \space\space \square 
\\]  

## Cardinalità di insiemi 
### def 
Si dice che due insiemi \\( A, B \\) hanno la stessa **cardinalità** (o _potenza_) se è possibile stabilire tra essi una funzione bigettiva.\\( \space\space \square  \\).   

### proposizione 
Due insiemi che hanno la stessa cardinalità sono in relazione di equivalenza tra loro, tale relazione si dice _di equipotenza_.   
Indichiamo che due insiemi \\( A, B \\) sono equipotenti, così

\\[
A \mathrel{\sim} B \iff |A| = |B|
\\]

### def 
Un insieme \\( A \\) si dice **finito** se per qualche \\( n \in \mathbb{N}, n \neq 0 \implies |A| = |I_n| \\) dove \\( I_n = \\{0, 1, 2, ..., n-1\\} \\) si dice **infinito**, altrimenti. \\( \space\space \square  \\)

## Cardinalità finite e infinite 
Nel caso di insiemi finiti, il concetto di cardinalità coincide con il numero di elementi che l'insieme contiene.   
Nel caso di insiemi infiniti utilizziamo delle specifiche notazioni. 

### def 
Un insieme si dice avere la **potenza del numerabile**, indicato con \\( \aleph_0 \\), se può essere messo in corrispondenza biunivoca con \\( \mathbb{N} \\). \\( \space\space \square  \\)

### corollario
Risulta immediato che insiemi finiti ed insiemi infiniti che possono essere correlati biunivocamente ad \\( \mathbb{N} \\) sono tutti insiemi numerabili.

### esempi 
Hanno cardinalità \\( \aleph_0 \\) gli insiemi \\( \mathbb{N}, \mathbb{Z}, \mathbb{Q} \\). Nel caso di \\( \mathbb{R} \\), invece, si parla di **potenza del continuo**

### def 
Chiamiamo **potenza del continuo** il numero cardinale \\( \mathfrak{c} = |\mathbb{R}| \space\space \square \\)

### proprietà 
Risulta (si veda più avanti) che \\( \aleph_0 \lt \mathfrak{c} \\), in altre parole la cardinalità di \\( \mathbb{R} \\) non è numerabile.

### teorema 
L'unione di un numero finito oppure di una infinità numerabile di insiemi numerabili ha la potenza del numerabile.

### dim 
Sia \\( A_1, A_2,\dots, A_j,\dots \\) una infinità numerabile di _insiemi numerabili_ a **due a due disgiunti**. 

ovvero:
\\[
  A_h \cap A_k = \emptyset, \forall h, k \in [1, n] \mid h \neq k
\\]  

Gli elementi del j-esimo insieme saranno:
\\[
  a_{j, 1}, a_{j, 2},...,a_{j, i},...
\\]  

Numeriamo adesso gli elementi di \\( A = \bigcup\limits_{h=1}^n A_h \\) per farlo disponiamo gli elementi di ogni insieme \\( A_h \\) su una tabella alla j-esima riga corrispondono gli elementi \\( a_{j, i} \in A_j \\):
\\[
\begin{array}{cccccc}
A_1 & a_{1,1} & a_{1,2} & a_{1,3} & \dots & a_{1,i} & \dots \\\\
A_2 & a_{2,1} & a_{2,2} & a_{2,3} & \dots & a_{2,i} & \dots \\\\
A_3 & a_{3,1} & a_{3,2} & a_{3,3} & \dots & a_{3,i} & \dots \\\\
\dots \\\\
A_j & a_{j,1} & a_{j,2} & a_{j,3} & \dots & a_{j,i} & \dots \\\\
\dots 
\end{array}
\\]  

Prendiamo la j-esima diagonale, ovvero:
\\[
  D_j = \\{ a_{h, k} \mid h + k = j + 1\\}
\\]
stabiliamo una corrispondenza biunivoca tra \\( A \\) ed \\( \mathbb{N} \\) considerando che ogni \\( a_{h, k} \in A \\) appartiene ad una sola diagonale, ovvero la \\( D_{h+k-1} \\), definiamo così la corrispondenza tra i due insiemi  
\\[
  a_{h, k} \mapsto 1 + 2 + 3 + \cdots + (h + k -2) + k
\\]
appare quindi evidente la corrispondenza bigettiva tra \\( A \\) ed \\( \mathbb{N} \\), segue che \\( A \\) sia numerabile. \\( \space\space \square  \\)

### teorema 
Dato un qualunque insieme numerabile \\( A \\), la cardinalità di tale insieme risulta sempre inferiore alla cardinalità del suo insieme delle parti:
\\[
  |A| < |\mathcal{P}(A)|
\\]
è infatti noto[^2] \\( |\mathcal{P}(A)| = 2^{\mathbb{N}} = \mathfrak{c} \\).


[^1]: M. Artin, _Algebra_, 1997 Bollati Boringhieri, p. 45.
[^2]: G.M. Piacentini Cattaneo, _Algebra, un approccio algoritmico_, 1996 Decibel, p. 35 e cfr. [anche](https://it.wikipedia.org/wiki/Cardinalit%C3%A0_del_continuo)
