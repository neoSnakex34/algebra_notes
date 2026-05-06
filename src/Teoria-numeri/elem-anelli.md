
# Introduzione sintetica agli anelli 
Si vogliono ora introdurre alcune definizioni inerenti al linguaggio dell'algebra astratta per mantenere un filo conduttore con la trattazione riguardante l'insieme \\( \mathbb{Z} \\). Determinate definizioni o proprietà sono di interesse anche nella teoria dei numeri. 

## Anello 
### Def  
Si chiama anello la struttura algebrica composta dalla tripla \\( R, +, \cdot \\) dove R è un insieme che gode di due operazioni binarie, somma e prodotto. Valgono le seguenti caratteristiche: 
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
In particolare (si veda capitolo successivo) \\( \(R, +) \\) è un **gruppo abeliano** e per il prodotto valgono la proprietà **distributiva** rispetto alla somma e la proprietà **associativa**. Nel caso in cui esista un elemento neutro per il prodotto, lo si dice elemento \\( 1 \\) (talvolta indicato con \\( e_1 \\) per specificare che sia l'elemento neutro) e si parla di **anello unitario**, nel caso in cui valga la proprietà commutativa per il prodotto, ovvero \\( \(R, \cdot\) \\) sia un gruppo abeliano, si parla allora di **anello commutativo**. \\( \space\space \square  \\)

> **Nota:** \\( \mathbb{Z} \\) è un anello commutativo unitario.
>

> **Nota:** definizioni più rigorose saranno date nel capitolo su anelli e campi.
>

## Divisori dello zero 
### Def 
Sia \\( a \in R \\), dove \\( \(R, +, \cdot \) \\) è un anello commutativo, se \\( a \neq 0 \land \exists b \in R, b \neq 0 \text { t.c. } ab = 0 \\) si dice che \\( a \\) è un divisore dello zero. 
\\( \space\space \square  \\)
## Dominio di integrità 
### Def 
Chiamiamo **dominio di integrità** un'anello commutativo che non possiede divisori dello zero. \\( \space\space \square  \\)

> **Nota**: è facile vedere che \\( \mathbb{Z} \\) sia un dominio di integrità.
>
