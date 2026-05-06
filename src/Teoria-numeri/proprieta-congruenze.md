# Proprietà delle congruenze

## Cancellazione in \\( \mathbb{Z}_n \\)
### Proposizione 
Se \\( ac \equiv bc \pmod n, MCD(c, n) = 1 \implies a \equiv b \pmod n \\)

### Dim 
Da definizione di congruenza modulo si ottiene che \\( n \mid c(a - b) \\), dato che \\( (c, n) = 1 \implies \exists s, t \text{ t.c. } 1 = sc + tn\\) (cfr. [identità di Bezout](numeri_parte3.)). Moltiplicando per \\( (a - b) \\) entrambi i membri:  
\\( (a - b) = s\mathbf{c(a-b)} + tn(a - b) \\) dunque n divide il primo membro da defininizione e' il secondo che contiene \\( n \\). Segue che se \\( a \mid (a - b) \implies a \equiv b \pmod n \\). \\( \space\space \square  \\)

### Proposizione 
Si può generalizzare la proprietà precedente in \\( ac \equiv bc \pmod n \implies a \equiv b \pmod{\frac{n}{MCD(c, n)}}  \\)

## Proprietà inerenti i numeri primi
### Proposizione 
Per ogni numero primo \\( p \\) e per ogni \\( x, y \in \mathbb{Z} \\) vale:  
\\[
  (x + y)^p \equiv x^p + y ^p \pmod p
\\]

## Dim - trattazione intuitiva 
Risulta dalla definizione di potenza di un binomio:  
\\[
  (a + b)^p = a^p + \sum\limits_{k = 1}^{p-1} \binom{p}{k} a^{p-k}b^k +b^p
\\]  
Si nota che \\( \binom{p}{k} \\) è un multiplo di \\( p \\), dunque è congruente modulo \\( 0 \\) a \\( p \\). cfr. Piacentini Cattaneo p. 70.
