# Congruenze e loro applicazioni

## Def 
Si definisce congruenza modulo \\( n \\) la seguente relazione definita su \\( \mathbb{Z} \\):  
\\[
  a \equiv b \pmod n \iff a - b = nh 
\\]
per qualche \\( h \in \mathbb{Z} \\). \\( \space\space \square  \\)

## Proposizione
Ogni \\( a \in \mathbb{Z} \\) è congruo modulo \\( n \\) ad un \\( r \in \mathbb{Z} \\), \\( 0 \le r \lt n \\).  

## Proposizione 
Per \\( n \gt 0, n \in \mathbb{Z} \\), la relazione \\( \equiv \\) è una relazione di equivalenza e valgono le seguenti proprietà:  
\\[
\begin{align}
& a, b, c, d \in \mathbb{Z} \newline
& a \equiv b \pmod n, c \equiv d \pmod n \implies 
  \begin{cases} 
  a + c \equiv b + d \pmod n \newline
  ac \equiv bd \pmod n
  \end{cases}
\end{align}
\\]

### Dim - primo caso 
\\( a \equiv b \pmod n \iff a - b = hn, c \equiv d \pmod n \iff c - n = kn  \\) dunque \\( a + c -(b + d) = n(h+k) \implies a + c \equiv b + d \pmod n \\). \\( \space\space \square  \\)

### Dim - secondo caso 
\\( ac - bd = ac - ad + bd = a(c - d) + d(a - b) = akn + hnd = n(ak + hd) \\) e quindi \\( ac \equiv bd \pmod n \\). \\( \space\space \square  \\)
