# Relazioni matematiche 

## Relazione
### Def
Una relazione tra due insiemi \\(A, B\\) è un sottoinsieme del loro prodotto cartesiano  
\\[\rho \subseteq A \times B\\]
si indicherà che la coppia \\( (a,b) \in \rho \\) con la notazione \\(a  \mathrel{\rho}  b. \space\space \square \\)  

## Relazione Inversa 
### Def 
Se \\( \mathrel{\rho} \\) è una relazione da \\( A \\) a \\( B \\), la relazione **inversa** \\( \mathrel{\rho}^{-1} \\) è la relazione[^1]
da \\( B \\) ad \\( A \\) definita da:
\\[
  b \mathrel{\rho^{-1}} a \iff a \mathrel{\rho} b. \space\space \square 
\\]
## Relazione di equivalenza {#rel_eq}
Considerando \\( \rho \\), una generica relazione di equivalenza definita sull'insieme \\( A \\).
### Def 
Se valgono le seguenti proprietà:
- **riflessività**: \\( a \mathrel{\rho} a, \forall a \in A \\) 
- **simmetria**: \\( a \mathrel{\rho} b \implies b \mathrel{\rho} a, \forall a, b \in A \\) 
- **transitività**: \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in A \\)  

allora si parla di **relazione di equivalenza**, indicata con \\( \sim. \space\space \square  \\)

## Classi di equivalenza modulo 
### Def 
Sia \\( \mathrel{\rho} \\) una relazione di equivalenza definita su \\( A \\). Si chiama **classe di equivalenza modulo \\( \mathrel{\rho} \\)** di un 
elemento \\( a \in A \\), indicata come \\( [a] \\), l'insieme di tutti gli elementi di \\( A \\) che sono equivalenti ad \\( a \\):
\\[
  [a] \overset{\text{def}}{=} \\{ b \in A \mid b \mathrel{\rho} a\\}  \space\space \square 
\\]  

> **Nota:** talvolta le classi di equivalenza sono scritte anche come \\( [a]_\sim \\) per indicare la specifica relazione di equivalenza a cui si riferiscono. 
### Proposizione 
Sia \\( \mathrel{\rho} \\) una relazione di equivalenza definita su \\( A \\). Allora:
\\[
  [a] = [b] \iff a \mathrel{\rho} b
\\]

### Teorema 
Sia \\( \mathrel{\rho} \\) una relazione di equivalenza in \\( A \\). Le classi di equivalenza di \\( A \\) modulo \\( \mathrel{\rho} \\) costituiscono una 
[_partizione_](https://it.wikipedia.org/wiki/Partizione_(teoria_degli_insiemi)) di \\( A \\)

## Insieme quoziente {#insieme_quoziente}
### Def 
Si dice **insieme quoziente** di \\( A \\) rispetto ad una data relazione di equivalenza \\( \alpha \\) l'insieme dato da tutte le classi di equivalenza modulo la relazione. 
Ovvero:  
\\[
  A/\alpha \overset{\text{def}}{=} \\{ [a]_\alpha \mid a \in A \\}
\\]

### Teorema 
Le classi di equivalenza di una data relazione \\( \alpha \\) definita su \\( A \\) partizionano l'insieme \\( A \\).

### Dim 
cfr. Piacentini Cattaneo p. 15 

### Teorema 
Una partizione di \\( A \\) determina su di esso una relazione di equivalenza, i sottoinsiemi della partizione risultano essere le sue classi di equivalenza 

### Dim 
cfr. Piacentini Cattaneo p. 15 

## Sul concetto di partizione 
Bisogna prestare attenzione ad intendere partizione nel senso [insiemistico](https://it.wikipedia.org/wiki/Partizione_(teoria_degli_insiemi)) del termine. 

### Def 
Sia \\( A \\) un generico insieme, una sua **partizione** è una divisione in sottoinsiemi che soddisfa le seguenti proprietà:

\\[
  \begin{align}
  (i)& \\ X_k \neq \emptyset \\ \forall X_k \mid X_k \subseteq X\\\\
  (ii)& \\ \bigcup\limits_{h=1}^n X_h = X\\\\
  (iii)& \\ X_i \cap X_j = \emptyset, \forall i, j \mid i \neq j
  \end{align}
\\]
\\( \space\space \square  \\)

<!--TODO esempi-->

## Relazioni d'ordine 
Si consideri \\( \rho \\), una generica relazione d'ordine definita su un insieme \\( A \\).
### Def
Se valgono le seguenti proprietà:
- **riflessività**: \\( a \mathrel{\rho} a, \forall a \in A \\) 
- **antisimmetria**: \\( a \mathrel{\rho} b \mathrel{\land} b \mathrel{\rho} a \implies a = b, \forall a,b \in A\\)
- **transitività**: \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in A \\)
  
allora si parla di **relazione d'ordine (parziale)**, indicata con \\( \le. \space\space \square \\)

> **Nota:** una relazione d'ordine in cui vale anche 
> - **totalità** \\( a \mathrel{\rho} b \lor b \mathrel{\rho} a, \forall a,b \in A \\)
> è detta **di ordine totale**, indicata con \\( \lt. \space\space \square \\)


[^1]: G.M Piacentini Cattaneo, _Algebra, un approccio algoritmico_, 1996 Decibel, p.13
