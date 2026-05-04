# Introduzione 

## Relazioni 
### def
Una relazione tra due insiemi \\(A, B\\) è un sottoinsieme del loro prodotto cartesiano  
\\[\rho \subseteq A \times B\\]
si indicherà che la coppia \\( (a,b) \in \rho \\) con la notazione \\(a  \mathrel{\rho}  b. \space\space \square \\)  

## Relazioni Inverse 
### def 
Se \\( \mathrel{\rho} \\) è una relazione da \\( A \\) a \\( B \\), la relazione **inversa** \\( \mathrel{\rho}^{-1} \\) è la relazione[^1]
da \\( B \\) ad \\( A \\) definita da:
\\[
  b \mathrel{\rho^{-1}} a \iff a \mathrel{\rho} b. \space\space \square 
\\]
## Relazioni di equivalenza {#rel_eq}
Considerando \\( \rho \\), una generica relazione di equivalenza definita sull'insieme \\( A \\).
### def 
Se valgono le seguenti proprietà:
- **riflessività**: \\( a \mathrel{\rho} a, \forall a \in A \\) 
- **simmetria**: \\( a \mathrel{\rho} b \implies b \mathrel{\rho} a, \forall a, b \in A \\) 
- **transitività**: \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in A \\)  

allora si parla di **relazione di equivalenza**, indicata con \\( \sim. \space\space \square  \\)

## Classi di equivalenza modulo 
### def 
Sia \\( \mathrel{\rho} \\) una relazione di equivalenza definita su \\( A \\). Si chiama **classe di equivalenza modulo \\( \mathrel{\rho} \\)** di un 
elemento \\( a \in A \\), indicata come \\( [a] \\), l'insieme di tutti gli elementi di \\( A \\) che sono equivalenti ad \\( a \\):
\\[
  [a] \overset{\text{def}}{=} \\{ b \in A \mid b \mathrel{\rho} a\\}  \space\space \square 
\\]  

> **Nota:** talvolta le classi di equivalenza sono scritte anche come \\( [a]_\sim \\) per indicare la specifica relazione di equivalenza a cui si riferiscono. 
### proposizione 
Sia \\( \mathrel{\rho} \\) una relazione di equivalenza definita su \\( A \\). Allora:
\\[
  [a] = [b] \iff a \mathrel{\rho} b
\\]

### teorema 
Sia \\( \mathrel{\rho} \\) una relazione di equivalenza in \\( A \\). Le classi di equivalenza di \\( A \\) modulo \\( \mathrel{\rho} \\) costituiscono una 
[_partizione_](https://it.wikipedia.org/wiki/Partizione_(teoria_degli_insiemi)) di \\( A \\)

## Insieme quoziente {#insieme_quoziente}
### def 
Si dice **insieme quoziente** di \\( A \\) rispetto ad una data relazione di equivalenza \\( \alpha \\) l'insieme dato da tutte le classi di equivalenza modulo la relazione. 
Ovvero:  
\\[
  A/\alpha \overset{\text{def}}{=} \\{ [a]_\alpha \mid a \in A \\}
\\]

### teorema 
Le classi di equivalenza di una data relazione \\( \alpha \\) definita su \\( A \\) partizionano l'insieme \\( A \\).

### dim 
cfr. Piacentini Cattaneo p. 15 

### teorema 
Una partizione di \\( A \\) determina su di esso una relazione di equivalenza, i sottoinsiemi della partizione risultano essere le sue classi di equivalenza 

### dim 
cfr. Piacentini Cattaneo p. 15 

## sul concetto di partizione 
Bisogna prestare attenzione ad intendere partizione nel senso [insiemistico](https://it.wikipedia.org/wiki/Partizione_(teoria_degli_insiemi)) del termine. 

### def 
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
### def
Se valgono le seguenti proprietà:
- **riflessività**: \\( a \mathrel{\rho} a, \forall a \in A \\) 
- **antisimmetria**: \\( a \mathrel{\rho} b \mathrel{\land} b \mathrel{\rho} a \implies a = b, \forall a,b \in A\\)
- **transitività**: \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in A \\)
  
allora si parla di **relazione d'ordine (parziale)**, indicata con \\( \le. \space\space \square \\)

> **Nota:** una relazione d'ordine in cui vale anche 
> - **totalità** \\( a \mathrel{\rho} b \lor b \mathrel{\rho} a, \forall a,b \in A \\)
> è detta **di ordine totale**, indicata con \\( \lt. \space\space \square \\)

## Funzioni
### def
Si da il nome di **funzione** a quel particolare tipo di relazione matematica tra un insieme \\( A \\) detto **dominio** (l'insieme di partenza) e un insieme \\( B \\) detto **codominio** (l'insieme di arrivo) dove ogni elemento di \\( A \\) è associato ad **un solo** elemento di \\( B \\).  
Indichiamo la funzione con \\[
f: A \to B
\\] l'elemento \\( x \in A\\) associato da \\( f \\) al codominio è scritto \\( f(x)=y \in B \\) ed è detto immagine dell'elemento \\( x \\), talvolta indicata con \\( Im(x) \\).
\\( \space\space \square  \\)


## Proprietà delle funzioni 
### def
Si dice che una **funzione** \\( f: A \to B \\) è: 
 - **iniettiva**: se \\( \forall a, a' \in A, f(a) = f(a') \implies a = a' \\), detta anche __in__. \\( \space\space \square  \\)
 - **surgettiva**: se \\( Im(f) = B \\), detta anche __su__. \\( \space\space \square  \\)
 - **bigettiva**: se è sia __in__ che __su__, detta anche __biunivoca__. \\( \space\space \square  \\)

 > **Nota:** esistono svariati sinonimi ed aggettivi equivalenti per indicare 
  iniettività, suriettività e biiettività. 
  Ad esempio iniezione, suriezione, biiezione, bigezione,  surgezione ecc. Da ora in avanti si useranno in maniera intercambiabile.
  >> *Appunto*: i termini **su** e **in** sono abbastanza arcaici e poco utilizzati ad oggi, è inoltre importante notare che la definizione stessa di funzione possiede due connotati leggermente differenti, a noi interessa quello più comune dove insieme di partenza e di arrivo sono ben specificati.
 >
## Composizione di funzioni
### def
Considerate due funzioni \\( f: A \to B, g: B \to C\\) è possibile comporle in una terza funzione, detta funzione composta:
\\[
  g \circ f: A \to C
\\]
vale \\( (g \circ f)(a) \overset{\text{def}}{=} g(f(a)) \space \forall a \in A.  \space\space \square  \\)

[^1]: G.M Piacentini Cattaneo, _Algebra, un approccio algoritmico_, 1996 Decibel, p.13
