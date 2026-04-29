# Insiemi Numerici 

## Numeri Naturali \\( \mathbb{N} \\)
Sia \\( \mathbb{N} \\) = {0, 1, 2, ...} l'insieme dei numeri naturali, diamo - attraverso gli _assiomi di peano_ - 
la definizione formale di tale insieme.

### def
Data la terna \\( (\mathbb{N}, \sigma, 0)  \\), in cui \\( \mathbb{N} \\) è un insieme, \\( \sigma \\colon \mathbb{N} \to \mathbb{N}  \\) è un'applicazione e \\( 0  \in \mathbb{N}\\)  
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

### esempi 
- Addizione in \\( \mathbb{Z} \\)
\\[
  \\begin{aligned}
  +\colon \mathbb{Z} \times \mathbb{Z} &\to \mathbb{Z} \\\\
  (a, b) &\mapsto a \mathbin{+} b
  \\end{aligned}
\\]  

dove \\( c \overset{\text{def}}{=} a + b \\)  
con \\( a, b, c \in \mathbb{Z} \\)

- Unione tra sottoinsiemi 
\\[
  \\begin{aligned}
  \cup\colon \mathcal{P}(X) &\times \mathcal{P}(X) \to \mathcal{P}(X) \\\\
  (A, B) &\mapsto A \cup B
  \\end{aligned}
\\]  

dove \\( X \\) è un insieme, \\( \mathcal{P}(X) \\) è l'insieme delle parti;  
\\( C \overset{\text{def}}{=} A \cup B \\)  
e vale \\( A, B, C \in \mathcal{P}(X) \\)

## Struttura algebrica 
### def 
Chiamiamo **struttura algebrica** l'oggetto matematico composto da un insieme \\( S \\) che gode di 
una o più _operazioni n-arie_ che soddisfano determinati assiomi. 

## Operazioni definite su \\( \mathbb{N} \\)
Tramite gli assiomi di Peano possiamo definire su \\( \mathbb{N} \\) due operazioni binarie. 

### Somma
#### def
Comunque presi \\( n, m \in \mathbb{N} \\), allora vale
\\[
\begin{aligned}
n \mathbin{+} m \overset{\text{def}}{=} 
\begin{cases} 
\underbrace{\sigma(\sigma(\cdots \sigma}_{m \text{ volte}}(n))) & \text{se } m > 0 \\\\
n & \text{se } m = 0 
\end{cases}
\end{aligned}
\\]  
\\( \space.\space \square  \\)  
il numero \\( n \mathbin{+} m \\) è detto _somma_ di \\( n \\) ed \\( m \\).

#### corollario
Dalla definizione di cui sopra segue:  
\\( \sigma(n) = n \mathbin{+} 1 \\) dove l'elemento \\( 1 = \sigma(0) \\).

### Prodotto
#### def 
Comunque presi \\( n, m \in \mathbb{N} \\), allora vale 
\\[
\begin{aligned}
n \cdot m \overset{\text{def}}{=}
\begin{cases}
\underbrace{n + n + \dots + n}_{m \text{ volte}} & \text{se } m > 0 \\\\
0 & \text{se } m = 0
\end{cases}
\end{aligned}
\\]
\\( \space.\space \square  \\)  
il numero \\( n \mathbin{\cdot} m \\) è detto _prodotto_ di \\( n \\) ed \\( m \\).

## Principio del buon ordinamento  
### trattazione intuitiva
