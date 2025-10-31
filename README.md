# 🌊 Esercitazione “Wave Runup e rilievo fotogrammetrico costiero”  
### Repository per docenti e tutor universitari

---

## 🎯 Scopo della repository

Questa repository fornisce a docenti e tutor un **pacchetto completo di esercitazione integrata** per corsi universitari di **Scienze Ambientali**, **Geomorfologia costiera**, **Ingegneria marittima** o **Geografia fisica**.

L’attività è progettata come **simulazione realistica di incarico tecnico**: gli studenti operano come un gruppo di consulenza incaricato di stimare l’ingressione del runup costiero durante un evento di mareggiata estrema.  

Il progetto unisce componenti **teoriche**, **pratiche** e **comunicative**, sviluppando competenze quantitative e professionali.

---

## 🧩 Struttura della repository

```text
├── Capitolato Tecnico.pdf          → Documento ufficiale della “commessa”: specifiche operative e criteri di valutazione
├── LICENSE                         → Licenza d’uso open source (CC BY-NC-SA 4.0)
├── Ortofoto e DEM/                 → Materiali del rilievo fotogrammetrico (Borghetto S. Spirito)
│   ├── Digital_Elevation_Model.tif
│   ├── Ortofotomosaico.tif
│   ├── Rapporto tecnico drone.pdf
│   └── Report di elaborazione.pdf
├── Presentazione_per_studenti.docx → Breve introduzione motivazionale e istruzioni operative per la classe
├── README.md                       → Documento di riferimento per i docenti
├── Risorse/
│   ├── Lista tutorial disponibili.docx → Elenco e link ai video tutorial (Colab, QGIS, scrittura tecnica)
│   └── Manuale scrittura.pdf          → Linee guida per la redazione del report tecnico-scientifico
├── Source_files_Latex/
│   ├── Report rilievo fotogrammetrico/
│   │   ├── main.tex, tau.cls, tauenvs.sty, tau.bib → Template completo in LaTeX del report tecnico
│   └── capitolato_tecnico.tex          → Sorgente LaTeX del documento principale (per eventuali adattamenti)
└── Wave_Runup/
    ├── Dati_originali/
    │   ├── Tide_Gauge.csv
    │   └── Wave_buoy.csv
    └── wave_runup_model.ipynb          → Notebook didattico per l’analisi del runup in Google Colaboratory
```

## 📘 Contenuti e approccio didattico

L’esercitazione è costruita per favorire un apprendimento **attivo e realistico**, ispirato alle dinamiche di una **commessa professionale**.  
Gli studenti lavorano come consulenti incaricati di analizzare un evento di mareggiata e stimarne il runup massimo, utilizzando dati reali e strumenti scientifici.

### 🔹 Struttura del percorso

L’attività si articola in quattro componenti principali:

1. **Documentazione tecnica**
   - Il documento *Capitolato Tecnico* costituisce l’unico riferimento ufficiale, come in un incarico reale.
   - Include obiettivi, tempistiche, criteri di valutazione e regole operative.
   - Nessuna istruzione aggiuntiva viene fornita al di fuori del capitolato, per stimolare autonomia e capacità di interpretazione.

2. **Analisi dati e modellazione**
   - Il notebook `wave_runup_model.ipynb` guida passo passo gli studenti nella lettura dei dati e nell’applicazione di diversi modelli empirici di runup.
   - Le celle in Markdown forniscono spiegazioni teoriche e richiami alle basi di programmazione in Python e all’uso di Colaboratory.
   - L’analisi si conclude con la selezione di un valore rappresentativo di runup per la mappatura GIS.

3. **Geoprocessing e rappresentazione spaziale**
   - I risultati quantitativi ottenuti dal notebook vengono integrati in **QGIS**, utilizzando il DEM e l’ortofoto del rilievo fotogrammetrico.
   - Gli studenti producono una **mappa di rischio costiero**, individuando le aree soggette a potenziale inondazione.

4. **Comunicazione tecnico–scientifica**
   - L’esercitazione si conclude con la redazione di un **report tecnico** (max 5 pagine), seguendo il *Manuale di scrittura tecnico-scientifica* incluso nella cartella `Risorse/`.
   - Il report deve essere strutturato in modo coerente, tracciabile e basato su dati quantitativi.

---

### 🎓 Competenze sviluppate

| Area di competenza | Obiettivi formativi specifici |
|---------------------|--------------------------------|
| **Analisi costiera** | Applicare e confrontare modelli empirici di runup in contesti reali. |
| **Fotogrammetria** | Comprendere il flusso di lavoro di acquisizione e generazione di ortofoto e DEM. |
| **GIS e rappresentazione spaziale** | Visualizzare e interpretare i risultati in ambiente QGIS. |
| **Comunicazione tecnico-scientifica** | Redigere relazioni tecniche chiare, sintetiche e verificabili. |
| **Soft skills professionali** | Lavorare in gruppo, gestire scadenze e responsabilità in autonomia. |

---

### 💡 Filosofia didattica

> “Tutto ciò che serve è già nel capitolato tecnico.”  
>  
> L’esercitazione spinge gli studenti a **leggere, comprendere e tradurre un problema reale** in un approccio quantitativo.  
> L’obiettivo non è solo ottenere un risultato numerico, ma **adottare un metodo professionale** basato su dati, rigore e collaborazione.

---

### 🧭 Output finale atteso

- Notebook completato e commentato su **Google Colaboratory**  
- Mappa di inondazione costiera in **QGIS**  
- Relazione tecnica in formato `.pdf` (max 5 pagine, con bibliografia)

---

### 📎 Materiali di supporto

- 📄 `Capitolato Tecnico.pdf` – documento ufficiale della commessa  
- 📘 `Risorse/Manuale scrittura.pdf` – guida alla redazione del report  
- 🧾 `Risorse/Lista tutorial disponibili.docx` – elenco dei video tutorials 
- 🧱 `Source_files_Latex/` – template completo in LaTeX per la relazione tecnica

---

## 🎯 Obiettivi formativi

L’esercitazione è progettata per sviluppare competenze tecniche, metodologiche e trasversali coerenti con i profili formativi dei corsi di **Scienze Ambientali** e discipline affini.  
L’obiettivo non è solo applicare formule o strumenti, ma **ragionare come professionisti** che devono produrre risultati affidabili, tracciabili e comunicabili.

---

### 🔹 Competenze disciplinari

| Ambito | Obiettivi specifici |
|---------|--------------------|
| **Oceanografia e dinamica costiera** | Comprendere i meccanismi di runup e setup durante eventi di mareggiata estrema. |
| **Analisi ambientale quantitativa** | Applicare modelli empirici per stimare l’inondazione costiera e valutarne l’incertezza. |
| **Telerilevamento e fotogrammetria** | Utilizzare dati da rilievo drone per derivare ortofoto e modelli digitali del terreno (DEM). |
| **GIS e cartografia tematica** | Integrare dati raster e vettoriali per produrre mappe di rischio costiero. |
| **Scrittura tecnico-scientifica** | Redigere un report sintetico e verificabile, utilizzando terminologia e convenzioni professionali. |

---

### 🔹 Competenze trasversali

| Area | Obiettivi formativi |
|------|----------------------|
| **Autonomia operativa** | Organizzare e gestire un progetto tecnico a partire da un documento di incarico. |
| **Collaborazione** | Lavorare in gruppo, distribuendo ruoli e responsabilità in modo efficace. |
| **Problem solving** | Identificare criticità nei dati e proporre soluzioni coerenti con i vincoli tecnici. |
| **Comunicazione scientifica** | Presentare risultati con grafici, mappe e testo chiaro e tracciabile. |
| **Etica professionale** | Rispettare i principi di trasparenza, citazione delle fonti e correttezza metodologica. |

---

### 💬 In sintesi

> L’obiettivo formativo principale è far vivere agli studenti un’esperienza **autentica di lavoro tecnico-scientifico**, in cui la conoscenza teorica è messa alla prova in un contesto realistico e interdisciplinare.

Alla fine dell’attività, ogni studente sarà in grado di:

- leggere e interpretare un **capitolato tecnico** come base operativa di un incarico;
- elaborare dati reali in ambiente **Python/Colaboratory**;
- integrare risultati quantitativi in **QGIS**;
- comunicare i propri risultati con un **report professionale** conforme agli standard tecnico-scientifici.

---

## ⚖️ Licenza d’uso

Tutti i materiali contenuti in questa repository — dati, notebook, testi e template — sono distribuiti con licenza  
**Creative Commons Attribution – Non Commercial 4.0 International (CC BY-NC 4.0)**.

### 📋 Condizioni principali

- ✅ **Attribuzione obbligatoria:** deve essere sempre citato l’autore originale e la fonte del materiale.  
- 🚫 **Uso non commerciale:** il materiale può essere usato, modificato e distribuito liberamente **solo per scopi didattici o di ricerca non commerciale**.  
- 🔁 **Adattamento consentito:** i docenti possono riutilizzare e modificare i contenuti per i propri corsi, mantenendo la stessa licenza.  

Per maggiori dettagli, consultare il testo completo della licenza su  
👉 [creativecommons.org/licenses/by-nc/4.0](https://creativecommons.org/licenses/by-nc/4.0/)

> 💡 In breve: potete liberamente usare, adattare e condividere questo materiale per la didattica universitaria, a condizione di citare l’autore e non trarne profitto economico diretto.

---

## 👤 Autore

**Autore:** Alessio Rovere  
**Affiliazione:** Università Ca’ Foscari Venezia – Via Torino 155, 30172 Venezia  

### 📚 Riconoscimenti

Il materiale è stato sviluppato come parte delle attività di supporto alla didattica universitaria in ambito ambientale e costiero, con l’obiettivo di favorire la diffusione di pratiche didattiche **open**, **replicabili** e **orientate al metodo scientifico**.

> _“La scienza aperta comincia in aula: condividere strumenti e metodi è il primo passo per formare professionisti consapevoli.”_
