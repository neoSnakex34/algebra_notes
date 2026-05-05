# Insieme \\( \mathbb{Z} \\) dei numeri interi 

## Costruzione di \\( \mathbb{Z} \\) partendo da \\( \mathbb{N} \\)
Si definisca la [relazione di equivalenza](../Algebra-elementare/relazioni.md#rel_eq) \\( \rho \\) su \\( \mathbb{N} \times \mathbb{N} \\) nel modo seguente:
\\[
(n, m) \mathrel{\rho} (n', m') \iff n + m' = m + n'
\\]  
essendo \\( \rho \\) una relazione di equivalenza, essa **ripartisce** in classi di equivalenza l'insieme su cui è definita, si indicano tali classi come \\( \overline{(n, m)} \\).  
Si possono scegliere di usare come rappresentanti di queste classi degli elementi specifici:  
\\[
\begin{align}
  &(0, 0)\\\\
  &(1, 0),(2, 0),\dots,(n, 0)\\\\
  &(0, 1),(0, 2),\dots,(0, n) 
\end{align}
\\]
Si definisce, tramite questa costruzione, l'insieme \\( \mathbb{Z} \\) degli interi:
### def
\\[
\mathbb{Z} \overset{\text{def}}{=} \( \mathbb{N} \times \mathbb{N} \)/\rho 
\\]
Si ricorda che la notazione \\( S/\alpha \\) dove \\( S \\) è un insieme e \\( \alpha \\) è una relazione di equivalenza, indica un [insieme quoziente](introduzione.md#insieme_quoziente).
### def 
Risulta possibile dividere \\( \mathbb{Z} \\) in questo modo: 
\\[
\begin{align}
 \mathbb{Z}&^+ \overset{\text{def}}{=}  \\{ \overline{(n, 0)} \mid n \in \mathbb{N}, n \neq 0\\}\\\\
 &0 \overset{\text{def}}{=} \overline{(0, 0)}\\\\
 \mathbb{Z}&^- \overset{\text{def}}{=} \\{ \overline{(0, n)} \mid n \in \mathbb{N}, n \neq 0\\}
\end{align}
\\]  
prenderanno il nome di **interi positivi** gli elementi di \\( \mathbb{Z}^+ \\) e di **interi negativi** gli elementi di \\( \mathbb{Z}^- \\). \\( \space\space \square  \\)

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
Le due operazioni di cui sopra risultano **ben definite**[^1].

### def 
Si definiscono allora gli elementi di \\( \mathbb{Z} \\) come:  
\\[
  \begin{align}
  &\overline{(n, 0)} \overset{\text{def}}{=} n\\\\
  &\overline{(0, 0)} \overset{\text{def}}{=} 0\\\\
  &\overline{(0, n)} \overset{\text{def}}{=} -n
  \end{align}
\\].
\\( \space\space \square  \\)

## Proprietà valide in \\( \mathbb{Z} \\)
### valore assoluto 
#### def 
\\[
|x| \overset{\text{def}}{=} 
\begin{cases}
   x &\text{se } x \geq 0 \\\\
   -x & \text{se } x < 0
\end{cases}
\\]
\\( \space\space \square  \\)

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
Dalla definizione del prodotto in \\( \mathbb{Z} \\), definito sulle classi di equivalenza \\( \overline{(n, m)} \\), è possibile verificare le identità poste nel lemma.  
Per una spiegazione rigorosa si consulti Piacentini Cattaneo p. 44 o alternativamente Herstein p. 24 (ponendo particolare attenzione alle notazioni desuete). 

[^1]: I.N Herstein, _Algebra_, 1982 Editori Riuniti, p. 24
