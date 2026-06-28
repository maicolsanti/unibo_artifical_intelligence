# Analisi della Popolarità Fotografica tramite Metadati EXIF

Progetto sviluppato per il corso di **"Laboratorio di Ottimizzazione, Intelligenza Artificiale e Machine Learning"**.

L'obiettivo del progetto è determinare se i parametri tecnici di scatto scelti da un fotografo (sensibilità ISO, apertura del diaframma, tempo di esposizione, lunghezza focale) influenzano il successo e la popolarità di un'immagine su una piattaforma digitale.

## Come Ottenere il Dataset (Istruzioni per il Download)

I file dati originali non sono inclusi nel repository GitHub in quanto superano i limiti di dimensione fissati dalla piattaforma (> 100 MB).

Per poter eseguire correttamente il codice del notebook e scaricare i file del dataset necessari, seguire questi passaggi:

1. **Scarica l'archivio:** Collegati alla pagina ufficiale dell'**Unsplash Dataset** (versione *Lite*) o cliccare sul seguente [link](https://unsplash.com/data/lite/latest).
2. **Estrai i file:** Estrai l'archivio ZIP sul tuo computer.
3. **Posiziona i file nel progetto:** Copia e incolla il file `photos.csv000` all'interno della **cartella assets di questo repository**.

## Requisiti e Installazione

Prima di avviare il notebook, assicurarsi di avere installato l'ambiente Python e le librerie necessarie. Si possono installare eseguendo il seguente comando nel terminale:

```bash
pip install -r requirements.txt
```