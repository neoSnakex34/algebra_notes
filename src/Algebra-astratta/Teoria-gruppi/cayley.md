# Tabelle di Cayley
Si può rappresentare un gruppo tramite una tavola di composizione, detta anche **tabella di Cayley** o tabella moltiplicativa.

## Struttura 
Sia \\( (G, \star) \\) un generico gruppo con una generica legge di composizione star definita su esso, allora la tabella di Cayley per \\( (G, \star) \\) è così costruita:  

| \\( \star \\) | \\( g_1 \\) | \\( g_2 \\) | \\( \cdots \\) | \\( g_j \\) | \\( \cdots \\) | \\( g_n \\) |
|---|---|---|---|---|---|---|
| \\( g_1 \\) | \\( g_1 \star g_1 \\) | \\( g_1 \star g_2 \\) | \\( \cdots \\) | \\( g_1 \star g_j \\) | \\( \cdots \\) | \\( g_1 \star g_n \\) |
| \\( g_2 \\) | \\( g_2 \star g_1 \\) | \\( g_2 \star g_2 \\) | \\( \cdots \\) | \\( g_2 \star g_j \\) | \\( \cdots \\) | \\( g_2 \star g_n \\) |
| \\( \vdots \\) | \\( \vdots \\) | \\( \vdots \\) | \\( \ddots \\) | \\( \vdots \\) | \\( \ddots \\) | \\( \vdots \\) |
| \\( g_i \\) | \\( g_i \star g_1 \\) | \\( g_i \star g_2 \\) | \\( \cdots \\) | \\( g_i \star g_j \\) | \\( \cdots \\) | \\( g_i \star g_n \\) |
| \\( \vdots \\) | \\( \vdots \\) | \\( \vdots \\) | \\( \ddots \\) | \\( \vdots \\) | \\( \ddots \\) | \\( \vdots \\) |
| \\( g_n \\) | \\( g_n \star g_1 \\) | \\( g_n \star g_2 \\) | \\( \cdots \\) | \\( g_n \star g_j \\) | \\( \cdots \\) | \\( g_n \star g_n \\) |

## Proprietà
Dato che nei gruppi abeliani l'operazione è commutativa, è facile verificare se un gruppo è abeliano guardando la sua tabella di Cayley. Se la tavola è simmetrica rispetto alla diagonale principale, il gruppo è abeliano.

## esempi
### \\( (\mathbb{Z}_4, +) \\)
\\( \mathbb{Z}_4 = \{0, 1, 2, 3\} \\)

| + | 0 | 1 | 2 | 3 |
|:---:|:---:|:---:|:---:|:---:|
| 0 | 0 | 1 | 2 | 3 |  
| 1 | 1 | 2 | 3 | 0 |  
| 2 | 2 | 3 | 0 | 1 |  
| 3 | 3 | 0 | 1 | 2 |
