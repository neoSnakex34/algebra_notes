# Insiemi Numerici 

## Numeri Naturali \\( \mathbb{N} \\)
Sia \\( \mathbb{N} \\) = {0, 1, 2, ...} l'insieme dei numeri naturali, diamo - attraverso gli _assiomi di peano_ - 
la definizione formale di tale insieme.

### def
Data la terna \\( (\mathbb{N}, \sigma, 0)  \\), in cui \\( \mathbb{N} \\) è un insieme, \\( \sigma : \mathbb{N} \to \mathbb{N}  \\) è un'applicazione e \\( 0  \in \mathbb{N}\\)  
Valgono le seguenti condizioni:
- \\( \mathbb{N}_1 \\): \\( \sigma \\) è iniettiva.
- \\( \mathbb{N}_2 \\): \\( 0 \notin Im(\sigma) \\)
- \\( \mathbb{N}_3 \\): ogni sottoinsieme \\( U \\) di \\( \mathbb{N} \\) tale che:
  - (a): \\( 0 \in U \\)
  - (b): \\( k \in U \implies \sigma(k) \in U \space \forall k \\)  

  coincide con tutto \\( \mathbb{N} \\)

l'elemento \\( \sigma(n) \\) è detto **successivo** di \\( n \\);  
il postulato \\( \mathbb{N}_3 \\) è detto principio di [_induzione matematica_](https://it.wikipedia.org/wiki/Principio_d%27induzione)
\\( \space.\space \square  \\)

## Operazione binaria 
### def 
Un'applicazione \\( S: S \times S \to S \\) è detta **operazione binaria** (anche[^1] _legge di composizione_, nella fattispecie **interna**), ossia una legge che associa ad ogni 
coppia \\( (a, b) \in S \\) un ben determinato elemento di \\( S  \space.\space \square \\)
> **Nota**: si parla di legge di composizione **esterna** nel caso \\( R \times S \to S \mid R \ne S \\) 
>
[^1]: M. Artin, _Algebra_, 1997 Bollati Boringhieri, p. 45.
