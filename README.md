# 🧠 Visual KNN Classifier (`k = 1`)

Questo codice HTML/JavaScript implementa un **classificatore visivo K-Nearest Neighbors (KNN)** con `k = 1`, utilizzabile direttamente in un browser.

## 🔍 Funzionamento

- L'utente può **cliccare sul canvas**:
  - **Tasto sinistro**: aggiunge un punto rosso (classe 0)
  - **Tasto destro**: aggiunge un punto blu (classe 1)
- I punti vengono salvati in un array con coordinate e label.
- Premendo il bottone “Allena modello”, il sistema colora lo sfondo del canvas in base alla **classificazione KNN con `k = 1`** per ogni pixel.

## 📊 Algoritmo

Il classificatore utilizza il **Nearest Neighbor algorithm**, ovvero il caso particolare di KNN dove `k = 1`.  
Per ogni punto (pixel), il modello assegna l'etichetta del punto addestrato più vicino in base alla distanza euclidea.

> Secondo Wikipedia:
>
> > "In the **k-nearest neighbors algorithm (k-NN)**, the output is a class membership. An object is classified by a majority vote of its neighbors, with the object being assigned to the class most common among its k nearest neighbors."  
> > — [Wikipedia: k-nearest neighbors algorithm](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)

Nel caso `k = 1`, viene assegnata direttamente l’etichetta del punto più vicino.

## 📁 File coinvolto

Il comportamento è definito nel file `classificatore.html`, completamente autonomo e senza dipendenze esterne.
