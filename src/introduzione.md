# Introduzione 

## Relazioni 
### Def
Una relazione tra due insiemi \\(A, B\\) è un sottoinsieme del loro prodotto cartesiano  
\\[\rho \subseteq A \times B\\]
indichiamo che la coppia \\( (a,b) \in \rho \\) come \\(a  \mathrel{\rho}  b \\).  
### Relazioni di equivalenza
se valgono le seguenti proprietà:
- [riflessività] \\( a \mathrel{\rho} a, \forall a \in \rho \\) 
- [simmetria] \\( a \mathrel{\rho} b \implies b \mathrel{\rho} a, \forall a, b \in \rho \\) 
- [transitività] \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in \rho \\)  

allora si parla di **relazione di equivalenza**, indicata con \\( \sim \\)

<!--TODO esempi-->

### Relazioni d'ordine 
se valgono le seguenti proprietà:
- [riflessività] \\( a \mathrel{\rho} a, \forall a \in \rho \\) 
- [antisimmetria] \\( a \mathrel{\rho} b \mathrel{\land} b \mathrel{\rho} a \implies a = b, \forall a,b \in \rho\\)
- [transitività] \\( a \mathrel{\rho} b, b \mathrel{\rho} c \implies a \mathrel{\rho} c, \forall a,b,c \in \rho \\)
  
allora si parla di **relazione d'ordine (parziale)**, indicata con \\( \le \\)

> **Nota:** una relazione d'ordine in cui vale anche 
> - [totalità] \\( a \mathrel{\rho} b \lor b \mathrel{\rho} a, \forall a,b \in \rho\\)
> è detta **di ordine totale**, indicata con \\( \lt \\)

## Funzioni
### Def
chiamiamo **funzione** un particolare tipo di relazione matematica tra un insieme \\( A \\) detto **dominio** e un insieme \\( B \\) detto **codominio** dove ogni elemento di \\( A \\) è associato ad un solo elemento di \\( B \\).  
Indichiamo la funzione con \\[
f: A \to B
\\] l'elemento \\( x \in A\\) associato da \\( f \\) al codominio è scritto \\( f(x)=y \in B \\) ed è detto immagine dell'elemento \\( x \\).

### Notazioni 
> si considerino i seguenti punti come definizioni
>

diciamo che una **funzione** \\( f: A \to B \\) è: 
 - [iniettiva] se \\( \forall a, a' \in A, f(a) = f(a') \implies a = a' \\), detta anche __in__
 - [surgettiva] se \\( Im(f) = B \\), detta anche __su__ 
 - [bigettiva] se è sia __in__ che __su__, detta anche __biunivoca__

### Composizione di funzioni
considerate due funzioni \\( f: A \to B, g: B \to C\\) definiamo la loro composizione come:
\\[
  g \circ f: A \to C
\\]
vale \\( (g \circ f)(a) \overset{\text{def}}{=} g(f(a)) \space \forall a \in A  \space .\square \\)
