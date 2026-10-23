# Metodi Iterativi, Gradiente Coniugato ed Equazioni Normali

Questo progetto sviluppa e analizza metodi iterativi per la risoluzione di sistemi lineari $Ax = b$ e problemi ai minimi quadrati tramite equazioni normali, con un focus approfondito sulle tecniche di accelerazione della convergenza tramite precondizionamento in ambiente MATLAB.

## Contenuto della Repository

* **`progetto_gradiente.pdf`**: Report completo generato dal Live Script, contenente il quadro teorico, il codice, i grafici di convergenza e i risultati sperimentali già renderizzati (consultabile direttamente senza eseguire il codice).
* **`progetto_gradiente.mlx`**: Live Script MATLAB eseguibile per riprodurre o estendere i test numerici.


## Contenuto del Progetto

Il Live Script (`progetto_gradiente.mlx`) (visibile anche nel  implementa e confronta le seguenti metodologie numeriche:

1. **Metodo del Gradiente (Steepest Descent):**
   * Implementazione dell'algoritmo classico per matrici simmetriche e definite positive.
   * Analisi del fattore di riduzione dell'errore legato al numero di condizionamento $\mathcal{K}(A)$.

2. **Metodo del Gradiente Coniugato (CG):**
   * Implementazione del metodo $CG$ per la minimizzazione del funzionale quadratico.
   * Monitoraggio dell'andamento dei residui $r_k = b - A x_k$ e dell'errore nella norma $A$.
   * Studio della convergenza teorica ed effettiva in funzione dello spettro dei valori propri.

3. **Metodo del Gradiente Coniugato Precondizionato (PCG):**
   * Introduzione di precondizionatori per ridurre il numero di condizionamento della matrice del sistema.
   * Confronto del numero di iterazioni necessarie per raggiungere la tolleranza prefissata rispetto al CG classico.

4. **Risoluzione di Equazioni Normali:**
   * Applicazione dei metodi iterativi (CG e PCG) alla risoluzione di sistemi sovradeterminati e problemi ai minimi quadrati $A^T A x = A^T b$.
   * Analisi dell'impatto della quadratura del numero di condizionamento $\mathcal{K}(A^T A) = \mathcal{K}(A)^2$ sulle prestazioni e sulla stabilità numerica.

## Requisiti e Tecnologie
* **MATLAB** 
* MATLAB Live Editor per l'esecuzione e la visualizzazione interattiva dei file `.mlx`

## Esecuzione
Aprire ed eseguire il file `progetto_gradiente.mlx` all'interno dell'ambiente MATLAB Live Editor per visualizzare l'analisi e i grafici generati.

## Autore
* **Giulia Reverberi**
