# Toziente di Eulero, piccolo teorema di Fermat

## Funzione toziente 
### def 
Per \\( n > 1 \\) si definisce la funzione \\( \phi \\), detta toziente o _funzione di Eulero_ dove \\( \phi(n) = x \text{ t.c. } x = Card(\\{y \lt n \mid MCD(n, y) = 1\\}) \\)

## Piccolo teorema di Fermat 
### Teorema 
Presi \\( a \in \mathbb{Z} \\) e un numero primo \\( p \\) vale la seguente congruenze:  
\\[
  a^p \equiv a \pmod p 
\\]

### dim - trattazione intuitiva 
Si può procedere per induzione su \\( a \\). Cfr. Piacentini Cattaneo, p. 70.

### corollario
Se \\( (a, p) = 1 \\) vale, ovviamente
\\[
  a^{p - 1} \equiv 1 \pmod p
\\]

## Teorema di eulero
Si nota che la funzione toziente è una generalizzazione del piccolo teorema di Fermat nella forma vista nel corollario precedente.

### Teorema 
Vale questo risultato:
\\[
  a^{\phi(n)} \equiv 1 \pmod n 
\\]
Se \\( \phi(p) = p - 1 \\)

### proposizione 
Presa una fattorizzazione di \\( n  = p_1^{h_1} p_2^{h_2} \cdots p_s^{h_s} \\) in numeri primi distinti. Si vuole dimostrare che per \\( \phi(n) \\) valga la proprietà di moltiplicatività.

#### funzione moltiplicativa 
##### def 
Si dice moltiplicativa quella funzione \\( f \\) in cui vale \\( f(rs) = f(r) f(s) \\). \\( \space\space \square  \\)
