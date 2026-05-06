# Teorema fondamentale dell'aritmetica
## Teorema 
Ogni numero intero \\( n > 1 \\) è un numero primo oppure è esprimibile (_può essere fattorizzato in_) come prodotto di numeri primi. _Al netto dell'ordine_ tale scrittura è **unica**.  

Il teorema viene diviso in due sottoenunciati per comodità dimostrativa[^1]. 
### Primo enunciato - esistenza della fattorizzazione
\\\( \forall a \in \mathbb{Z}_{\ge 2}, \exists b = p_1^{\alpha_1}p_2^{\alpha_2} \dots p_t^{\alpha_t} \mid b = a \\).  
Dove \\( p_1 > p_2 > p_3, \dots \\) sono numeri primi ed ogni \\( \alpha_i > 0 \\)

### Secondo enunciato - unicità della fattorizzazione 
La rappresentazione di \\( a \\) espressa come \\( b \\) nel primo enunciato è unica. 

### Dim - esistenza 
Si procede per induzione (e conseguente equivalenza con il principio del buon ordinamento)
- passo base: \\( \(a = 2\) \\), \\( 2 \\) è **primo** \\( \implies b = p_i^{a_i} = 2 \\)
- ipotesi induttiva:  \\( \forall r \in \mathbb{Z} \mid 2 \le r \le n \\) vale il primo enunciato
- passo induttivo: data per vera l'ipotesi induttiva fino ad \\( n \\) si procede su \\( n + 1 \\). 
  - se \\( n + 1  \\) è primo, l'enunciato è vero. 
  - se \\( n + 1 \\) non è primo, è divisibile per un primo \\( p \\) questo implica che \\( \exists m = \(n + 1 \)/p\\) è ovviamente minore di \\( n + 1 \\) ma ogni numero minore di \\( n + 1 \\) verifica l'enunciato per ipotesi induttiva. Segue che \\( \(n + 1) = mp \\) è fattorizzabile. 

\\(  \space\space \square \\)

### Dim - unicità
Si vuole procedere per induzione sul numero \\( m \\) di fattori primi.
- passo base: (\\( m = 1\\)) fattori  
Se \\( n \\) ha \\( m = 1 \\) come numero di fattori \\( \implies m \\) è primo, \\( p > 1 \\).  
Si suppone che \\( n = p \\) abbia una seconda fattorizzazione \\( p = q_1^{\beta_1}q_2^{\beta_2}\dots  q_h^{\beta_h} \\), con \\( q_i > 1 \\). Se \\( p \\) è una fattorizzazione, deve (per il lemma di euclide) dividere un elemento al secondo membro, diciamo \\( p \mid q_i \\) e applichiamo la legge di cancellazione in \\( \mathbb{Z} \\) semplificando \\( p \\).  
\\[
  1 = q_1^{\beta_1}q_2^{\beta_2}\dots q_i^{\beta_i - 1} \dots  q_h^{\beta_h}
\\]  
Dall'equazione di cui sopra segue che ogni \\( \beta_i = 0 \\) altrimenti l'identità non sarebbe verificata. Ne segue direttamente che 
\\[
  p = q_i
\\] 
è l'unica fattorizzazione di \\( n \\).  

- ipotesi induttiva: l'unicità vale per ogni fattorizzazione lunga \\( m - 1 \\) elementi.  
- passo induttivo: \\( n  \\) ha una fattorizzazione lunga \\( m \\) elementi.  
  sia
\\[
    n = p_1^{\alpha_1}p_2^{\alpha_2}\dots p_i^{\alpha_i} = 
q_1^{\beta_1}q_2^{\beta_2}\dots q_h^{\beta_h} 
\\]  
con \\( p_l, q_m \gt 1 \\) entrambi numeri primi una rappresentazione di **due** distinte fattorizzazioni per \\( n \\). Il numero di fattori (la somma degli esponenti) di sinistra è \\( m \\), ma essendo entrambe fattorizzazioni di \\( n \\), un fattore \\( p_i \\) divide un fattore \\( q_i \\), per legge di cancellazione si ottiene una fattorizzazione di \\( m - 1 \\) fattori a sinistra, che è unica per ipotesi induttiva, segue che i fattori \\( q_i \\) coincidano con quelli di sinistra a meno dell'ordine. \\( \space\space \square  \\)



[^1]: cfr. I.N. Herstein, _Algebra_, 1982 Editori Riuniti, pp.21, 22.
