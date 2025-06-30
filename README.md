# 🏠 RealEstateAI Solutions

## 📌 Obiettivo del Progetto

**RealEstateAI Solutions** si propone di ottimizzare la valutazione dei prezzi immobiliari attraverso l'uso di **tecniche avanzate di regolarizzazione** in modelli di regressione lineare.

L’obiettivo principale è fornire **previsioni di prezzo più accurate e affidabili**, riducendo il rischio di overfitting e migliorando la capacità di generalizzazione del modello. In un mercato immobiliare sempre più competitivo, questo sistema rappresenta uno strumento strategico per agenti e investitori.

---

## 📊 Dataset Utilizzato

Il dataset, liberamente disponibile, è accessibile al seguente link:
* Dataset: [housing.csv](https://proai-datasets.s3.eu-west-3.amazonaws.com/housing.csv)  
* Ispirato al dataset Kaggle: [Housing Prices Dataset](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset)

### 🧾 Variabili presenti:

| Variabile         | Descrizione |
|------------------|-------------|
| `Price`          | Prezzo dell’immobile (**target**) |
| `Area`           | Superficie |
| `Bedrooms`       | Numero di camere da letto |
| `Bathrooms`      | Numero di bagni |
| `Stories`        | Numero di piani |
| `Mainroad`       | 1 se affaccia su una strada principale, 0 altrimenti |
| `Guestroom`      | 1 se ha una stanza degli ospiti, 0 altrimenti |
| `Basement`       | 1 se ha un seminterrato, 0 altrimenti |
| `Hotwaterheating`| 1 se ha una caldaia, 0 altrimenti |
| `Airconditioning`| 1 se ha aria condizionata, 0 altrimenti |
| `Parking`        | Numero di parcheggi |
| `Prefarea`       | 1 se situato in una zona prestigiosa, 0 altrimenti |
| `Furnishingstatus` | 0 = non arredato, 1 = parzialmente arredato, 2 = completamente arredato |

---

## ⚙️ Tecnologie e Librerie Utilizzate

- Python 
- Pandas & NumPy
- Scikit-learn
- Seaborn & Matplotlib

---

## 🧪 Fasi del Progetto

### 1. **Preparazione del Dataset**
- Caricamento dei dati
- Gestione dei valori mancanti
- Codifica di eventuali variabili categoriche
- Normalizzazione/standardizzazione dei dati

### 2. **Implementazione dei Modelli**
- Regressione **Ridge**
- Regressione **Lasso**
- Regressione **Elastic Net**

Tutti i modelli sono stati implementati utilizzando **Cross Validation automatica** (con `RidgeCV`, `LassoCV`, `ElasticNetCV`)

### 3. **Valutazione delle Performance**
- Calcolo del **Mean Squared Error (MSE)**
- Calcolo del **R² score**
- Analisi della complessità del modello tramite il **numero di coefficienti non nulli**

### 4. **Visualizzazione dei Risultati**
- Grafici di confronto tra i modelli
- Visualizzazione dei residui
- Curve di apprendimento (learning curve)

---

## 📈 Risultati e Conclusioni

Il confronto tra i metodi di regolarizzazione ha evidenziato che:

- **Ridge** regge bene nei casi con multicollinearità
- **Lasso** permette la selezione automatica delle feature
- **Elastic Net** combina i vantaggi di entrambi i metodi

Grazie alla regolarizzazione, si è ottenuto un **modello più robusto e generalizzabile**, riducendo significativamente l’overfitting rispetto alla regressione lineare standard

---

## 👨‍💻 Autore

**Giacomo Latini**  
Master in AI Engineering - ProfessionAI
![image](https://github.com/user-attachments/assets/8df6a8a9-4d40-40d0-995b-35638b72a538)

---

## 📂 Come eseguire il progetto

1. Clona la repository:

```bash
git clone https://github.com/tuo-username/realestate-ai-solutions.git
cd realestate-ai-solutions
```
