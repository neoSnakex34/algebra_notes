
#  brevi elementi di teoria degli Anelli 
Introduciamo delle definizioni inerenti al linguaggio dell'algebra astratta per mantenere un filo conduttore con l'insieme \\( \mathbb{Z} \\). Determinate definizioni o proprietà sono di interesse anche nella teoria dei numeri. 

## Anello 
### def  
Si chiama anello la struttura algebrica composta dalla tripla \\( R, +, \cdot \\) dove R è un insieme e le operazioni binarie su esso definite, spesso chiamate somma e prodotto, hanno specifiche proprietà:
\\[
  \begin{align}
  R \neq \emptyset \newline
  \newline
  +\colon R \times R& \to R \newline
  (a, b)& \mapsto a + b \newline
  \newline
  \cdot\colon R \times R& \to R \newline
  (a, b)& \mapsto ab \newline
  \end{align}
\\]   
In particolare (si veda capitolo successivo) \\( \(R, +) \\) è un **gruppo abeliano** e per il valgono la proprietà **distributiva** rispetto alla somma e la proprietà **associativa**. Nel caso in cui esista un elemento neutro per il prodotto, chiamiamo tale elemento \\( 1 \\) (talvolta indicato con \\( e_1 \\) per specificare che sia l'elemento neutro) e si parla di **anello unitario**, nel caso in cui valga la proprietà commutativa per il prodotto, ovvero \\( \(R, \cdot\) \\) sia un gruppo abeliano, parliamo allora di **anello commutativo**.

## divisori dello zero 
### def 
Sia \\( a \in R \\), dove \\( \(R, +, \cdot \) \\) è un anello commutativo, se \\( a \neq 0 \land \exists b \in R, b \neq 0 \text { t.c. } ab = 0 \\) diciamo che \\( a \\) è un divisore dello zero. 
\\( \space\space \square  \\)
## dominio di integrità 
### def 
Chiamiamo **dominio di integrità** un'anello commutativo che non possiede divisori dello zero. \\( \space\space \square  \\)

> **Nota**: è facile vedere che \\( \mathbb{Z} \\) sia un dominio di integrità.
>
