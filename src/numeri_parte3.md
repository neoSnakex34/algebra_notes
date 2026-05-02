# Teorema fondamentale dell'aritmetica
## Teorema 
Ogni numero intero \\( n > 1 \\) è un numero primo oppure è esprimibile (_può essere fattorizzato in_) come prodotto di numeri primi. _Al netto dell'ordine_ tale scrittura è **unica**.  

Il teorema viene diviso in due sottoenunciati per comodità dimostrativa[^1]. 
### primo enunciato - esistenza della fattorizzazione
\\\( \forall a \in \mathbb{Z}_{\ge 2}, \exists b = p_1^{\alpha_1}p_2^{\alpha_2} \dots p_t^{\alpha_t} \mid b = a \\).  
Dove \\( p_1 > p_2 > p_3, \dots \\) sono numeri primi ed ogni \\( \alpha_i > 0 \\)

### secondo enunciato - unicità della fattorizzazione 
La rappresentazione di \\( a \\) espressa come \\( b \\) nel primo enunciato è unica. 

### dim - esistenza 
Si procede per induzione (e conseguente equivalenza con il principio del buon ordinamento)
- passo base: \\( \(a = 2\) \\), \\( 2 \\) è **primo** \\( \implies b = p_i^{a_i} = 2 \\)
[^1]: cfr. I.N. Herstein, _Algebra_, 1982 Editori Riuniti, pp.21, 22.
- ipotesi induttiva:  \\( \forall r \in \mathbb{Z} \mid 2 \le r \le n \\) vale il primo enunciato
- passo induttivo: data per vera l'ipotesi induttiva fino ad \\( n \\) si procede su \\( n + 1 \\). 
  - se \\( n + 1  \\) è primo, l'enunciato è vero. 
  - se \\( n + 1 \\) non è primo, è divisibile per un primo \\( p \\) questo implica che \\( \exists m = \(n + 1 \)/p\\) è ovviamente minore di \\( n + 1 \\) ma ogni numero minore di \\( n + 1 \\) verifica l'enunciato per ipotesi induttiva. Segue che \\( \(n + 1) = mp \\) è fattorizzabile. 

\\(  \space\space \square \\)

### dim - unicità
**Hp**   
Esistono due distinte fattorizzazioni di un numero \\( a \\), siano
\\[
  \begin{align}
    \[1\]& \quad a = p_1^{\alpha_1}p_2^{\alpha_2}\dots p_i^{\alpha_i} \newline
    \[2\]& \quad a = q_1^{\beta_1}q_2^{\beta_2}\dots  q_h^{\beta_h} 
  \end{align}
\\]  
con \\( p_i^{\alpha_i} \neq q_h^{\beta_h} \\) entrambi numeri primi.
