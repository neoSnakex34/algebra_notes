# Immersione di un anello in un campo 
Rimandando le definizioni di quanto verrà adesso enunciato ai capitoli che riguarderanno gli argomenti di algebra astratta, si da una conclusione dell'argomento inerente il campo dei razionali. 

## Proposizione 
Il campo \\( \mathbb{Q} \\) rappresenta un'estensione di \\( \mathbb{Z} \\) tale che ogni elemento di \\( \mathbb{Q} \\) si può scrivere come \\( ab^{-1}, a, b \in \mathbb{Z} \land b \neq 0 \\). 

### Dim - trattazione intuitiva
Per dimostrare che \\( \mathbb{Q} \\) sia un'estensione di \\( \mathbb{Z} \\) si vuole mostrare come l'anello \\( \mathbb{Z} \\) possa essere _immerso_ nel campo \\( \mathbb{Q} \\), ovvero come i razionali formino il cosiddetto **campo dei quozienti** degli interi.  Per fare ciò si può definire una funzione: 
\\[ 
\begin{align}
\phi \colon &\mathbb{Z} \to \mathbb{Q} \newline 
 & a \mapsto \overline{(a, 1)}
\end{align}
\\]  
che risulta essere iniettiva (la dimostrazione di ciò è omessa), e si può verificare essere un omomorfismo iniettivo, notare questo è fondamentale per garantire che la struttura degli interi si conservi nei razionali.  
Si conclude osservando quindi che è possibile scrivere \\( \mathbb{Z} \subseteq \mathbb{Q} \\) e riferirsi agli elementi di \\( \mathbb{Q} \\) come \\( \frac{a}{b}\\). 

si veda Piacentini Cattaneo pp. 58, 59 per una trattazione rigorosa dell'argomento.

> **Nota importante:** l'applicazione \\( \phi \\) può anche essere espressa in termini di teoria delle categorie, non affrontata in questi appunti. In quel caso si parla di un morfismo iniettivo, ovvero un monomorfismo.
>
