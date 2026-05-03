# Immersione di un anello in un campo 
Rimandando le definizioni di quanto verrà adesso enunciato ai capitoli che riguarderanno gli argomenti di algebra astratta, si da una conclusione dell'argomento inerente il campo dei razionali. 

## proposizione 
Il campo \\( \mathbb{Q} \\) rappresenta un'estensione di \\( \mathbb{Z} \\) tale che ogni elemento di \\( \mathbb{Q} \\) si può scrivere come \\( ab^{-1}, a, b \in \mathbb{Z} \land b \neq 0 \\). 

### dim - trattazione intuitiva
Per dimostrare che \\( \mathbb{Q} \\) sia un'estensione di \\( \mathbb{Z} \\) si vuole mostrare come l'anello \\( \mathbb{Z} \\) possa essere _immerso_ nel campo \\( \mathbb{Q} \\), ovvero come i razionali formino il cosiddetto **campo dei quozienti** degli interi.  Per fare ciò si può definire un [**morfismo**](https://it.wikipedia.org/wiki/Immersione_(matematica)), ovverosia una funzione 
\\[ 
\begin{align}
\phi \colon &\mathbb{Z} \to \mathbb{Q} \newline 
 & a \mapsto \overline{(a, 1)}
\end{align}
\\]  
che risulta essere iniettivo (la dimostrazione di ciò è omessa), dunque un monomorfismo, notare questo è fondamentale per garantire che la struttura degli interi si conservi nei razionali.  
Si conclude osservando quindi che è possibile scrivere \\( \mathbb{Z} \subseteq \mathbb{Q} \\) e riferirsi agli elementi di \\( \mathbb{Q} \\) come \\( \frac{a}{b}\\). 

si veda Piacentini Cattaneo pp. 58, 59 per una trattazione rigorosa dell'argomento.

> **Nota importante:** il termine **morfismo** è di uso nella teoria delle categorie, non affrontata in questi appunti, viene utilizzato per questioni di eleganza di notazione in questo contesto. In termini più vicini all'algebra astratta si può parlare di omomorfismo iniettivo di anelli.
>
