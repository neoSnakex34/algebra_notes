# Divisioni di interi, MCD 
  
## divisione euclidea  
### def  
cfr. [Teorema 4.2](https://www.mat.uniroma2.it/~gavarini/page-web_files/mat-didat_data/dispense-ecc/note_di_D%27Andrea/Aritmetica.pdf)
\\[
  a, b \in \mathbb{Z} \text{ t.c. } b \neq 0 \implies \exists q, r \in \mathbb{Z}, a = qb + r, 0 \le r \lt |b|. 
\\]
\\( \space\space \square  \\)

## divisori
Si introduce ora la definizione formale di divisore, accennato nella definizione di dominio di integrità.
### def 
Se è possibile scrivere un elemento \\( c = ab, a, b, c \in \mathbb{Z} \\), ovvero se dalla definizione precedente risulta \\( r = 0 \\), allora si dice che \\( a \\) divide \\( b \\), e lo si indica con \\( a \mid b \\). Se tale numero non esiste allora si dice che \\( a \\) non divide \\( b \\) e lo si indica con \\( a \nmid b \\). \\( \space\space \square  \\)

## divisori comuni 
### def 
Viene definito **divisore comune** il numero \\( z \in \mathbb{Z} \\) per il quale esistono opportuni \\(  a, b \in \mathbb{Z} \\) tali che \\( z \mid a \land z \mid b \\). \\( \space\space \square  \\)

### proprietà 
Vale questo importante lemma:  
se tale divisore comune esiste, ovvero se \\( \exists z \in \mathbb{Z} \text{ t.c. } z \mid a \land z \mid b\\) allora \\( z \mid sa + tb, \forall s,t \in \mathbb{Z} \\).

### dim 
\\( z \\) è un divisore comune di \\( a, b \\), che significa che i numeri \\( a, b \\) possono essere scritti nella forma \\( c = ab \\).   
Dunque \\( a = zh, b = zk \\) per opportuni \\( h, k \in \mathbb{Z} \\).  
Risulta evidente che \\( \forall s, t \in \mathbb{Z}, sa + tb = s(zh) + t(zk) \\).  

Raccogliendo per \\( z \\) si ottiene:  
\\( sa + tb = s(zh) + t(zk) = z(sh + tk) \\) che essendo un numero moltiplicato per un coefficiente \\( z \\) risulta, ovviamente, \\( z \mid sa + tb \\). \\( \space\space \square  \\)

## Invertibili
### def 
Un numero \\( u \in \mathbb{Z} \\) che divide \\( 1 \\), ovvero per cui \\( 1 = uk \\) per opportuno \\( k \in \mathbb{Z} \\), si dice elemento **invertibile**.

> **Nota:** gli unici elementi invertibili in \\( \mathbb{Z} \\) sono \\( 1, -1 \\), mentre in strutture algebriche come i _campi_ ogni elemento a parte lo \\( 0 \\) è invertibile.
>

## Irriducibili e Primi 
### def 
Si dice **irriducibile** quell'elemento \\( z \in \mathbb{Z} \text{ t.c. } z \neq 0 \\) e che non è possibile scomporre in fattori, ovverosia se scrivendo \\( z = ab \\), risulta che \\( a \lor b \\) sono elementi invertibili. \\( \space\space \square  \\)

### def 
si dice **elemento primo** un elemento \\( z \in \mathbb{Z} \\) diverso dallo zero e dagli invertibili tale che se \\( z \mid ab \implies z \mid a \lor z \mid b \\). \\( \space\space \square  \\)

> **Nota:** in \\( \mathbb{Z} \\) elementi primi e elementi irriducibili coincidono.
>

## MCD 
### def 
Si dice **massimo comun divisore** di \\( a, b \in \mathbb{Z} \\), indicato con \\( MCD\(a, b\) \\) o più semplicemente con \\( \(a, b \) \\) quell'elemento \\( d \\) appartenente ad un generico _anello commutativo_ (in questo caso l'anello degli interi) in cui vale:  
\\[
  \begin{align}
  (&i)\\ d \mid a, d \mid b \newline
  (i&i)\\ z \mid a, z \mid b \implies z \mid d 
  \end{align}
\\]
\\( \space\space \square  \\)
> **Nota:** è bene notare che l'MCD non è unico, infatti se \\( d = \(a, b \) \\) anche \\( -d = \(a, b \) \\) ovvero un MCD moltiplicato per gli elementi invertibili dell'anello è ancora un MCD.

### numeri relativamente primi 
#### def 
Si dicono **relativamente primi** o _coprimi_ i due \\( a, b \in \mathbb{Z} \text{ t.c. } \(a, b \) = 1\\). \\( \space\space \square  \\)

### lemma di esistenza di MCD ed identità di Bezout
#### prima parte
Siano \\( a, b \in \mathbb{Z}, \\ a \neq 0 \lor b \neq 0  \implies \exists \(a, b \) \\).
#### seconda parte 
Si possono trovare due interi \\( n, m \\) per cui \\( \(a, b \) = na + mb \\)

> **Nota**: si utilizza il termine _combinazione lineare_, di solito di uso negli spazi vettoriali, per indicare una combinazione di due elementi di un anello \\( a, b \in R \\) per opportuni coefficienti \\( h, k \in \mathbb{Z} \\).
  >> _Appunto_: risulta evidente che i due interi \\( n, m \\) del lemma di cui sopra formino una combinazione lineare con \\( a, b \\). 
>

#### pre dimostrazione 
Si consideri un sottoinsieme \\( \mathbb{Z}^{li} \subset \mathbb{Z} \\) formato da interi esprimibili come combinazioni lineari di \\( a, b \\) su un anello (degli interi). Dal fatto che \\( a \\) o \\( b \\) non sono entrambi nulli segue che in questo insieme ci siano degli interi non nulli.
Siccome \\( n, m \\) spaziano su tutti gli interi, è ovvio che se un generico \\( z = na + mb \in \mathbb{Z}^{li} \\) anche \\( -z = \(-n\)a+ \(-n\)b \in \mathbb{Z}^{li} \\) è quindi possibile considerare una sezione di interi positivi su \\( \mathbb{Z}^{li} \\).  
Vale dunque il [principio del buon ordinamento](insiemi.md#buon_ordinamento), quindi  

**Hp**  
esiste un **minimo** intero positivo \\( c = na + mb \\).  

**Th**  
\\( c = \(a, b \) \\).  

#### dim
Sia \\( d \\) è un divisore comune di \\( a, b \\), per il lemma citato nella sezione dei divisori comuni, risulta \\( d \mid (na + mb) \implies d \mid c \\), resta da dimostrare che \\( c \\) sia un divisore comune per \\( a, b \\).  
Preso un qualunque elemento \\( x \overset{\text{def}}{=} n_sa + m_sb \in \mathbb{Z}^{li} \\) dalla la definizione di divisione euclidea risulta \\( x = qc + r, \\ 0 \le r \lt c \\). Esprimendo in maniera esplicita i numeri \\( x \\) e \\( c \\) si ottiene:  
\\( n_sa + m_sb = q \( na + mb \) + r \\), da cui segue che \\( r = a \( n_s - qn \) + b \( m_s - qm \) \\) ovvero \\( r \in \mathbb{Z}^{li} \\).  
Se \\( r \\) fosse maggiore di zero avremmo una **contraddizione** di quanto formulato in **Hp** segue che \\( r = 0 \\).  
Dunque \\( x = qc \\) che significa che c è un divisore di qualsiasi elemento \\( x \\) espresso come combinazione lineare, in particolare \\( x = a; \text{ se } n_s = 1, m_s = 0 \implies c \mid a \land x = b; \text{ se }  n_s = 0, m_s = 1 \implies c \mid b \\). Dato che \\( c \\) è un divisore comune ed è diviso da ogni altro divisore, risulta essere l'MCD\\( \space\space \square  \\)

#### conclusioni 
La scrittura di un MCD come combinazione lineare \\( na + mb \\) è chiamata **identità di Bezout**.

#### corollario 
Se \\( a, b \\) sono coprimi allora \\( 1 = na + mb \\) per opportuni \\( n, m \in \mathbb{Z} \\).

## Algoritmo Euclideo per MCD 
Si può utilizzare la tecnica di scrittura della divisione euclidea sugli interi in maniera consecutiva per trovare l'MCD tra due numeri.

### alg 
Siano \\( a, b \in \mathbb{Z}, a \ge b \gt 0 \\)  

\\[
\begin{align}
  &(1) \quad a = b q_{1} + r_1 \newline
  &(2) \quad b = r_1 q_{2} + r_2 \newline
  &(3) \quad r_1 = r_2 q_{3} + r_3 \newline
  &\qquad \vdots \newline 
  &(n) \quad r_{n-2} = r_{n - 1} q_n + \mathbf{r_n} \newline 
  &(n + 1) \quad r_{n-1 } = \mathbf{r_n} q_{n+1} + 0. 
\end{align}
\\]

In altre parole \\( MCD(a, b) \\) è l'ultimo resto non nullo nell'algoritmo.

## Algoritmo Euclideo esteso per identità di Bezout 
Risulta possibile scrivere in termini di \\( a, b \\) i resti delle divisioni applicate
nell'algoritmo base, così facendo possiamo trovare due numeri \\( \alpha, \beta \\) che formano un'identità di Bezout per \\( MCD(a, b) \\). 

### alg applicato ad un esempio 
Si vuole calcolare \\( (413, 173) \\)
#### algoritmo base
\\[
\begin{align}
  &(1) \quad 413 = 173(2) + 67  \newline
  &(2) \quad 173 = 67(2) + 39 \newline
  &(3) \quad 67 = 39(1) + 28 \newline
  &(4) \quad 39 = 28(1) + 11  \newline
  &(5) \quad 28 = 11(2) + 6  \newline
  &(6) \quad 11 = 6(1) + 5  \newline
  &(7) \quad  6 = 5(1) + \mathbf{1}  \newline
  &(8) \quad  5 = 1(5) + 0  \newline
\end{align}
\\]  

Risulta \\( MCD(413, 173) = 1 \\)

#### algoritmo esteso 
Si vuole ora trovare una identità di Bezout, è necessario provedere scrivendo i resti ottenuti dal precedente algoritmo in termini dei numeri \\( a, b \\).  
Si inizia riscrivendo gli \\( n \\) passi usati nell'agoritmo di base, al contrario, in termini dei resti:
\\[
  \begin{align}
  &(7) \quad \mathbf{1} = 6 - 5(1)  \newline
  &(6) \quad 5 = 11 - 6(1) \newline
  &(5) \quad 6 = 28 - 11(2) \newline
  &(4) \quad 11 = 39 - 28(1) \newline
  &(3) \quad 28 = 67 - 39(1) \newline
  &(2) \quad 39 = 173 - 67(2) \newline
  &(1) \quad 67 = 413 -173(2) \newline
  \end{align}
\\]  
Si costruisce dunque l'identità sviluppando i termini: 
\\[
\begin{align}
   1 = & \quad 6 - \[ 11 - 6(1) \] \newline
   1 = & \quad -11 + 6(2) \newline
   1 = & \quad -11 +\[ 28 - 11(2)\](2) \newline
   1 = & \quad -11(5) + 28(2) \newline
   1 = & \quad -\[39 - 28\](5) + 28(2) \newline
   1 = & \quad -39(5) +28(7) \newline
   1 = & \quad -39(5) +\[ 67 - 39(1)\](7) \newline
   1 = & \quad -39(12) + 67(7) \newline
   1 = & \quad -\[173 - 67(2) \](12) + 67(7) \newline
   1 = & \quad -173(12) +67(31) \newline
   1 = & \quad -173(12) +\[ 413 - 173(2)\](31)\newline
   1 = & \quad -173(74) + 413(31) \newline
  \newline 
   1 = & \quad 413(\mathbf{31}) + 173(\mathbf{-74}) \newline
\end{align}
\\]  

Segue che una identità di Bezout per l'MCD in questione è \\( x = 31, y = -74 \\)
