# Introduzione 

## Relazioni 
### def
Una relazione tra due insiemi \\(A, B\\) è un sottoinsieme del loro prodotto cartesiano  
\\[\rho \subseteq A \times B\\]
indichiamo che la coppia \\( (a,b) \in \rho \\) come \\(a  \mathrel{\rho}  b \space.\space \square \\)  

## Relazioni Inverse 
### def 
Se \mathrel{\rho} è una relazione da \\( A \\) a \\( B \\), la relazione **inversa** \\( \mathrel{\rho}^{-1} \\) è la relazione 
da \\( B \\) ad \\( A \\) definita da:
\\[
  b \mathrel{\rho^{-1}} a \iff a \mathrel{\rho} b \space.\space \square 
\\]
## Relazioni di equivalenza
### def 
se valgono le seguenti proprietà:
- [riflessività] \\( a \mathrel{\rho} a, \forall a \in \rho \\) 
- [simmetria] \\( a \mathrel{\rho} b \implies b \mathrel{\rho} a, \forall a, b \in \rho \\) 
- [transitività] \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in \rho \\)  

allora si parla di **relazione di equivalenza**, indicata con \\( \sim \space.\space \square  \\)

<!--TODO esempi-->

## Relazioni d'ordine 
### def
se valgono le seguenti proprietà:
- [riflessività] \\( a \mathrel{\rho} a, \forall a \in \rho \\) 
- [antisimmetria] \\( a \mathrel{\rho} b \mathrel{\land} b \mathrel{\rho} a \implies a = b, \forall a,b \in \rho\\)
- [transitività] \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in \rho \\)
  
allora si parla di **relazione d'ordine (parziale)**, indicata con \\( \le \space.\space \square \\)

> **Nota:** una relazione d'ordine in cui vale anche 
> - [totalità] \\( a \mathrel{\rho} b \lor b \mathrel{\rho} a, \forall a,b \in \rho\\)
> è detta **di ordine totale**, indicata con \\( \lt \space.\space \square \\)

## Funzioni
### def
chiamiamo **funzione** un particolare tipo di relazione matematica tra un insieme \\( A \\) detto **dominio** e un insieme \\( B \\) detto **codominio** dove ogni elemento di \\( A \\) è associato ad un solo elemento di \\( B \\).  
Indichiamo la funzione con \\[
f: A \to B
\\] l'elemento \\( x \in A\\) associato da \\( f \\) al codominio è scritto \\( f(x)=y \in B \\) ed è detto immagine dell'elemento \\( x \\)
\\( \space.\space \square  \\)
## Proprietà delle funzioni 
### def
diciamo che una **funzione** \\( f: A \to B \\) è: 
 - [iniettiva] se \\( \forall a, a' \in A, f(a) = f(a') \implies a = a' \\), detta anche __in__ \\( \space.\space \square  \\)
 - [surgettiva] se \\( Im(f) = B \\), detta anche __su__ \\( \space.\space \square  \\)
 - [bigettiva] se è sia __in__ che __su__, detta anche __biunivoca__ \\( \space.\space \square  \\)

## Composizione di funzioni
### def
considerate due funzioni \\( f: A \to B, g: B \to C\\) definiamo la loro composizione come:
\\[
  g \circ f: A \to C
\\]
vale \\( (g \circ f)(a) \overset{\text{def}}{=} g(f(a)) \space \forall a \in A  \space.\space \square  \\)
