# Aritmetica in \\( \mathbb{Z} \\) 
  
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

#### lemma di esistenza di MCD ed identità di Bezout
##### prima parte
Siano \\( a, b \in \mathbb{Z}, \\ a \neq 0 \lor b \neq 0  \implies \exists \(a, b \) \\).
##### seconda parte 
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
