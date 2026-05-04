# Teoria dei Gruppi

## Gruppo 
### def 
Si definisce **gruppo** la struttura algebrica definita dalla coppia \\( (G, \star) \\) in cui \\( G \\) è un insieme non vuoto e \\( \star \\) è un'operazione binaria così definita:  
\\[
  \begin{align}
    \star \colon &G \times G \to G \newline
    &(a, b) \mapsto a \mathop{\star} b
  \end{align}
\\]

La funzione \\( \star \\) gode delle seguenti caratteristiche:
- **associatività**: \\( (a \star b) \star c = a \star (b \star c) \ \forall a,b,c \in G \\)
- **elemento neutro**: \\( \exists e \in G \text{ t.c. } a \star e = e \star a = a \ \forall a,b,c \in G\\)
- **elemento inverso**: \\( \exists a^{-1} \in G \text{ t.c. } a \star a^{-1} = e \ \forall a,b,c \in G\\)
\\( \space\space \square  \\)

### Gruppo abeliano 
#### def 
Un gruppo dove valga anche:  
- **commutatività**: \\( a \star b = b \star a  \ \forall a,b,c \in G\\)
si dice **gruppo abeliano** o _commutativo_. \\( \space\space \square  \\)

> **Nota:** 
Generalmente le operazioni \\( \star \\) di interesse nella teoria dei gruppi sono la moltiplicazione o la composizione di funzioni, spesso si usa la notazione moltiplicativa \\( ab \\) invece di \\( a \star b \\). Da ora in avanti si usera la più snella notazione \\(  (G, \cdot) \\).  
L'elemento neutro quando non indicato con \\( e \\) sarà indicato come elemento neutro specifico per l'operazione, nel caso di \\( \cdot \\) l'elemento neutro è l'\\( 1 \\).
>
## Proprietà
### proposizione - unicità del neutro
Se \\( (G, \cdot) \\) è un gruppo \\( \exists! e \in G \\).

### dim 
**Hp** esistono due elementi neutri \\( e_1, e_2 \in G \\) rispetto alla sua operazione, risulta quindi \\( e_1g = ge_1 = g \\ \forall g \in G \\) ma anche \\( e_2g = ge_2 = g\\ \forall g \in G \\) è quindi possibile notare che: 
\\[
\begin{align}
  &e_1e_2 = e_2e_1 = e_2 \newline
  &e_2e_1 = e_1e_2 = e_1
\end{align}
\\]
Ne segue che \\( e_1 = e_2 \\). \\( \space\space \square  \\)

### proposizione - unicità degli inversi 
Se \\( (G, \cdot) \\) è un gruppo \\( \forall a \in G_{>0} \exists! a^{-1} \mid aa^{-1} = e \\). 

### dim 
Siano \\( a', a'' \\) due inversi di un dato elemento \\( a \in G \\), si può dunque scrivere:  
\\[
  a' = ea' = (a'' a)a' = a'' (aa') = a'' e = a''
\\]
risulta immediata l'uguaglianza. \\( \space\space \square  \\)

### corollario - inverso del prodotto 
Risulta quindi utile notare che \\( (ab)^{-1} = b^{-1}a^{-1} \\), infatti si può vedere:  
\\[
  (ab)\cdot b^{-1}a^{-1} = a(bb^{-1})a^{-1} = a(e)a^{-1} = aa^{-1} = e
\\]
che essendo un inverso per \\( (ab) \\) è l'unico, dalla dimostrazione precedente.

## Esempi
- \\( (\mathbb{Z}, +), (\mathbb{Q}, +), (\mathbb{R}, +) \\)
- Il gruppo generale lineare \\( (GL_n(\mathbb{K}), \cdot) \overset{\text{def}}{=} {A \in M_n(\mathbb{K})} \mid det A \neq 0 \\)
