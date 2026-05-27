# Analisi della Popolarità Fotografica tramite Metadati EXIF

Questo repository contiene il progetto sviluppato per il corso di **"Laboratorio di Ottimizzazione, Intelligenza Artificiale e Machine Learning"**.

L'obiettivo del progetto è determinare se i parametri tecnici di scatto scelti da un fotografo (sensibilità ISO, apertura del diaframma, tempo di esposizione, lunghezza focale) influenzano il successo e la popolarità di un'immagine su una piattaforma digitale. Il problema è affrontato come un task di **Classificazione Binaria** (Foto Popolare vs Non Popolare).

## Struttura del Notebook

1. **Introduzione del problema:** Inquadramento teorico del task e definizione della variabile target.
2. **Descrizione del dataset:** Analisi delle caratteristiche del campione di immagini.
3. **Lettura e preparazione dei dati:** Caricamento del dataset e gestione avanzata dei dati mancanti tramite tecniche di *Data Imputation* (sostituzione con la mediana per conservare la dimensionalità del dataset).
4. **Visualizzazione ed EDA:** Analisi esplorativa delle distribuzioni delle feature e studio delle correlazioni con la popolarità dello scatto.
5. **Outlier detection / preprocessing:** Identificazione e rimozione di anomalie fisiche o software nei parametri EXIF (es. valori incongruenti o corrotti) per garantire la robustezza dei modelli.
6. **Implementazione di uno o più modelli:** Addestramento di modelli di classificazione (es. Random Forest, Logistic Regression, Multi-Layer Perceptron) e ottimizzazione guidata degli iperparametri tramite ricerca su griglia (*GridSearchCV*).
7. **Valutazione e confronto dei risultati:** Analisi approfondita di metriche quali Accuracy, Precision, Recall, F1-Score e visualizzazione della Matrice di Confusione.
8. **Conclusioni finali:** Considerazioni sulla *feature importance* e sull'efficacia predittiva dell'approccio basato unicamente sui parametri tecnici.

## Come Ottenere il Dataset (Istruzioni per il Download)

In conformità con le direttive del corso (*"Qualora il Notebook non scarichi autonomamente il dataset da internet, fornire gli stessi nel repository o istruzioni per l'ottenimento in caso di grandi dimensioni"*), i file dati originali non sono inclusi nel repository GitHub in quanto superano i limiti di dimensione fissati dalla piattaforma (> 100 MB).

Per poter eseguire correttamente il codice del notebook e scaricare i file del dataset necessari, seguire questi passaggi:

1. **Scarica l'archivio:** Collegati alla pagina ufficiale dell'**Unsplash Dataset** (versione *Lite*) o cliccare sul seguente [link](https://unsplash.com/data/lite/latest).
2. **Estrai i file:** Estrai l'archivio ZIP sul tuo computer.
4. **Posiziona i file nel progetto:** Copia e incolla i file `.csv000` all'interno della **cartella assets di questo repository**.

## Requisiti e Installazione

Prima di avviare il notebook, assicurati di avere installato l'ambiente Python e le librerie necessarie per il calcolo scientifico e il machine learning. Puoi installarle eseguendo il seguente comando nel tuo terminale:

```bash
pip install -r requirements.txt
```