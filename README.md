# 🌊 Esercitazione GGG — Wave Runup e rilievo fotogrammetrico costiero

## 📘 Descrizione generale

Questa repository contiene tutti i materiali per l’esercitazione **“Analisi del runup ondoso e rilievo fotogrammetrico della spiaggia di Borghetto S. Spirito (SV)”**, pensata per corsi di **Scienze Ambientali** (livello Laurea Triennale, II anno).  
L’esercitazione è concepita come un’attività **learn-by-doing**: le studentesse e gli studenti lavorano come in una piccola commessa professionale, seguendo un *capitolato tecnico* e producendo un *report tecnico scientifico* finale.

Tutti i dati, notebook e modelli sono compatibili con **Google Colaboratory** e con software GIS come **QGIS**.

---

## 🎯 Obiettivi formativi

- Introdurre le basi della **modellazione del runup ondoso** su spiagge sabbiose.  
- Applicare metodi di **fotogrammetria da drone** per la ricostruzione del DEM e dell’ortofoto.  
- Sviluppare capacità di **analisi critica dei risultati**, collegando teoria e osservazioni.  
- Produrre un **report tecnico-scientifico** in stile professionale, seguendo linee guida di scrittura.

---

## 📂 Struttura della repository

```├── Capitolato Tecnico.pdf         → documento principale con le specifiche operative dell’esercitazione
├── LICENSE                        → licenza open source del materiale
├── Ortofoto e DEM/                 → prodotti del rilievo fotogrammetrico
│   ├── Digital_Elevation_Model.tif
│   ├── Ortofotomosaico.tif
│   ├── Rapporto tecnico drone.pdf
│   └── Report di elaborazione.pdf
├── Source_files_Latex/             → sorgenti LaTeX per il report fotogrammetrico e il capitolato tecnico
│   ├── Report rilievo fotogrammetrico/
│   │   ├── main.tex, tau.cls, tauenvs.sty, tau.bib, etc.
│   └── capitolato_tecnico.tex
└── Wave_Runup/                     → esercitazione su modelli empirici di runup
├── Dati_originali/
│   ├── Tide_Gauge.csv
│   └── Wave_buoy.csv
└── wave_runup_model.ipynb      → notebook da aprire in Google Colab```

---

## 🧩 Come usare i materiali

### 🔹 1. Preparazione su Google Drive e Colaboratory
1. Scaricare la cartella `Wave_Runup.zip` o la cartella `Dati_originali` dalla repository.  
2. Decomprimere i file e caricarli in una cartella personale di Google Drive.  
3. Aprire il notebook `wave_runup_model.ipynb` su **Google Colaboratory**.  
4. Seguire le istruzioni e i commenti in Markdown nel notebook per completare l’analisi.

> 💡 Tutto ciò che serve per svolgere l’esercitazione è nel *capitolato tecnico*.

---

### 🔹 2. Analisi e risultati
Nel notebook vengono implementati diversi **modelli empirici di runup**.  
Gli studenti sono guidati a confrontare i risultati, produrre grafici e infine selezionare un valore rappresentativo di runup da **mappare in QGIS** sul DEM o sull’ortofoto.

L’output finale previsto è una **relazione tecnica di max 5 pagine**, inclusa bibliografia.

---

## 🧾 Materiali di supporto

- 📄 **Capitolato tecnico** → regole e specifiche operative dell’esercitazione.  
- 📘 **Manuale di scrittura tecnico-scientifica** → [link da aggiungere qui]  
- 🎥 **Video tutorial Colaboratory e QGIS** → [link da aggiungere qui]  
- 📎 **Esempi di report fotogrammetrici e runup** → cartella `Source_files_Latex/`

---

## 🧑‍🏫 Per i docenti

Questa esercitazione è pensata per essere facilmente **adottabile in altri corsi** di geomorfologia costiera, geografia fisica o modellazione ambientale.  
Ogni componente (dati, notebook, testi) è riutilizzabile sotto licenza aperta.

### Adattabilità:
- Il notebook `wave_runup_model.ipynb` è interamente commentato e modificabile.  
- I file `.tif` del rilievo fotogrammetrico possono essere sostituiti da dati propri.  
- Il *capitolato tecnico* fornisce un modello replicabile di esercitazione basata su commessa.

---

## 🧠 Suggerimento didattico

L’esercitazione funziona al meglio se gli studenti lavorano in piccoli gruppi (2–3 persone), condividendo file e notebook su Google Drive.  
La discussione dei risultati e la redazione del report tecnico sono parti fondamentali dell’apprendimento.

---

## ⚙️ Requisiti tecnici

- Google Account con accesso a **Colaboratory**  
- **QGIS ≥ 3.30** (solo per la parte di mappatura)  
- Browser aggiornato (Chrome o Firefox consigliati)  

---

## 📄 Licenza

Questo materiale è distribuito sotto licenza **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)**.  
È consentito riutilizzarlo e modificarlo per fini didattici, citando la fonte.

---

## 📬 Contatti

**Autore:** Alessio Rovere  
**Affiliazione:** GeoDrone s.r.l. – Via Torino 155, 30172 Venezia  
**Email:** [aggiungere email accademica o di riferimento]

---

> _Questa repository nasce come supporto all’apprendimento attivo nelle scienze ambientali.  
> L’obiettivo è far vivere agli studenti un’esperienza di progetto reale, con strumenti e metodi professionali._