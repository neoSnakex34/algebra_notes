# Cenni di teoria dei numeri 
## Costruzione di \\( \mathbb{Z} \\) partendo da \\( \mathbb{N} \\)
Definita la [relazione di equivalenza](introduzione.md#rel_eq) \\( \rho \\) su \\( \mathbb{N} \times \mathbb{N} \\)  
\\[
(n, m) \mathrel{\rho} (n', m') \iff n + m' = m + n'
\\]  
è noto che l'insieme su cui abbiamo definito \\( \rho \\) viene **ripartito** in classi di equivalenza, che vogliamo indicare con \\( \overline{(n, m)} \\).  
Scegliamo di usare come rappresentanti di queste classi degli elementi specifici:  
\\[
\begin{align}
  &(0, 0)\\\\
  &(1, 0),(2, 0),\dots,(n, 0)\\\\
  &(0, 1),(0, 2),\dots,(0, n) 
\end{align}
\\]
Diamo una possibile definizione di \\( \mathbb{Z} \\):
### def
\\[
\mathbb{Z} \overset{\text{def}}{=} \( \mathbb{N} \times \mathbb{N} / \rho \) 
\\]
Ricordiamo che la notazione \\( S/\alpha \\) dove \\( S \\) è un insieme e \\( \alpha \\) è una relazione di equivalenza, indica un [insieme quoziente](introduzione.md#insieme_quoziente).
### def 
Possiamo dividere \\( \mathbb{Z} \\) in questo modo: 
\\[
\begin{align}
 \mathbb{Z}&^+ \overset{\text{def}}{=}  \\{ \overline{(n, 0)} \mid n \in \mathbb{N}, n \neq 0\\}\\\\
 &0 \overset{\text{def}}{=} \overline{(0, 0)}\\\\
 \mathbb{Z}&^- \overset{\text{def}}{=} \\{ \overline{(0, n)} \mid n \in \mathbb{N}, n \neq 0\\}
\end{align}
\\]  
chiamiamo **interi positivi** gli elementi di \\( \mathbb{Z}^+ \\) e **interi negativi** gli elementi di \\( \mathbb{Z}^- \\). \\( \space\space \square  \\)

## Operazioni definite su \\( \mathbb{Z} \\)
### Somma 
#### def
\\[
  \overline{(n, m)} + \overline{(n', m')} \overset{\text{def}}{=} \overline{(n + n', m + m')}
\\]

### Prodotto
#### def 

\\[
  \overline{(n, m)} \cdot \overline{(n', m')} \overset{\text{def}}{=} \overline{(nn' + mm', n'm + nm')}
\\]

### osservazione 
Le due operazioni che abbiamo definito risultano **ben definite**[^1].

### def 
Indichiamo allora gli elementi di \\( \mathbb{Z} \\) come:  
\\[
  \begin{align}
  &\overline{(n, 0)} \overset{\text{def}}{=} n\\\\
  &\overline{(0, 0)} \overset{\text{def}}{=} 0\\\\
  &\overline{(0, n)} \overset{\text{def}}{=} -n
  \end{align}
\\].
\\( \space\space \square  \\)

## Alcune proprietà di somma e prodotto 
### lemma 
Presi \\( a, b \in \mathbb{Z} \implies \\)  
\\[
  \begin{align}
  (i)& \\ a \cdot 0 = 0 \cdot a = 0\\\\ 
  (ii)& \\ (-a) \cdot b = -(a \cdot b)\\\\
  (iii)& \\ (-a) \cdot (-b) = a \cdot b 
  \end{align}
\\]

### dim intuitiva
dalla definizione del prodotto su \\( \mathbb{Z} \\) introdotto sulle classi di equivalenza \\( \overline{(n, m)} \\) si possono verificare le identità poste nel lemma.  
Per una spiegazione rigorosa si veda Piacentini Cattaneo p. 44 


[^1]: I.N Herstein, _Algebra_, 1982 Editori Riuniti, p. 24
