# 🌊 Esercitazione — Wave Runup e rilievo fotogrammetrico costiero

**Corso di Geografia Fisica e Geomorfologia — Laurea in Scienze Ambientali, Università Ca' Foscari Venezia (a.a. 2026/2027)**

---

## 🎯 Scopo

Questa repository contiene il materiale per un'esercitazione che simula un **incarico tecnico reale**: gli studenti, riuniti in gruppi, agiscono come una società di consulenza ambientale incaricata da un committente (GeoMarine Solutions/Engineering s.r.l.) di stimare la **massima ingressione del runup costiero** durante una mareggiata estrema sul litorale di Borghetto Santo Spirito (SV), e di mapparne le aree di potenziale inondazione.

L'unico riferimento operativo per gli studenti è il **Capitolato Tecnico** incluso nella repository: non vengono fornite istruzioni aggiuntive, per stimolare autonomia e capacità di interpretazione di un incarico professionale.

---

## 🧩 Struttura della repository

```text
├── Capitolato tecnico/
│   └── capitolato_tecnico.pdf          → Lettera di incarico ufficiale: obiettivi, dati forniti, attività richieste,
│                                          tempistiche, criteri di valutazione
├── Dati GNSS/                          → Rilievo RTK-GNSS del 12 maggio 2026, relativo alla mareggiata del 9-12 maggio 2026
│   ├── Punti_Sensibili_runup.csv         (punti di interesse/vulnerabilità sulla spiaggia)
│   ├── Runup_GNSS.csv                    (punti raggiunti dal runup durante l'evento)
│   ├── Transetto_GNSS.csv                (transetto topografico della spiaggia)
│   └── README_Dati_GNSS.pdf              (descrizione dei tre file: contenuto, uso previsto, sistema di riferimento)
├── Ortofoto e DEM/                     → Rilievo fotogrammetrico da drone dell'area di studio
│   ├── Digital_Elevation_Model.tif
│   ├── Ortofotomosaico.tif
│   ├── Rapporto tecnico drone.pdf
│   └── Report di elaborazione.pdf
├── Risorse/
│   ├── Manuale di Scrittura.pdf         → Linee guida per la redazione tecnico-scientifica del report
│   └── Bibliografia_di_riferimento.pdf  → Riferimenti scientifici sulla geomorfologia costiera dell'area e sul monitoraggio da drone
├── Wave_Runup/
│   └── esercitazione_wave_runup_costiero.ipynb  → Notebook (Google Colab) per il calcolo del runup
├── LICENSE                             → Licenza MIT
└── README.md
```

---

## 📘 Percorso didattico

L'attività si articola in tre fasi principali, descritte nel dettaglio nel Capitolato Tecnico.

**1. Calcolo del runup costiero — `Wave_Runup/esercitazione_wave_runup_costiero.ipynb`**
Il notebook (da eseguire su Google Colab) guida gli studenti attraverso:
- definizione di un punto di studio al largo e download di una serie storica di dati d'onda dal **Copernicus Marine Service**;
- esplorazione interattiva della serie per individuare una mareggiata significativa da modellizzare;
- recupero manuale dei dati di livello del mare per l'evento scelto dal portale **mareografico.it** (ISPRA);
- unione temporale di dati d'onda e marea;
- inserimento di valori di pendenza della spiaggia (tanβ);
- calcolo del runup con un **ensemble di 8 modelli empirici** (Stockdon et al. 2006, Vousdoukas et al. 2012, Holman 1986, Nielsen 2009, Ruggiero et al. 2001, Atkinson et al. 2017, Senechal et al. 2011, Passarella et al. 2018), tramite il pacchetto `py-wave-runup`;
- confronto statistico tra i modelli (istogrammi, percentili) e selezione di un valore rappresentativo di runup.

I dati raccolti in campo nella cartella `Dati GNSS/` (relativi alla stessa mareggiata, 9–12 maggio 2026) possono essere usati per verificare/confrontare criticamente i valori stimati dai modelli empirici — vedi `Dati GNSS/README_Dati_GNSS.pdf` per la descrizione dei tre file e indicazioni sul loro uso.

**2. Geoprocessing e mappatura — QGIS**
Utilizzando il DEM e l'ortofoto in `Ortofoto e DEM/` e il valore di runup scelto, gli studenti producono in QGIS una mappa delle aree potenzialmente soggette a inondazione costiera.

**3. Relazione tecnica**
Redazione di un report tecnico-scientifico (max 5 pagine, bibliografia esclusa), strutturato in Introduzione, Area di studio, Metodi e dati, Risultati e discussione, Conclusioni e raccomandazioni — secondo le linee guida in `Risorse/Manuale di Scrittura.pdf`. Un primo nucleo di riferimenti bibliografici pertinenti all'area di studio e ai metodi impiegati è disponibile in `Risorse/Bibliografia_di_riferimento.pdf`, da integrare con ulteriori fonti reperite autonomamente.

---

## 🗓️ Tempistiche (a.a. 2026/2027)

| Data | Attività |
|---|---|
| Novembre–Dicembre 2026 | Lavoro guidato in classe e con tutorial online |
| 30 novembre e 14 dicembre 2026 | Sessioni di lavoro in presenza (6 ore ciascuna) |
| 15 dicembre 2026, ore 23:59 | Consegna della relazione preliminare su Moodle |
| 21 dicembre 2026 | Revisione e discussione guidata |
| 15 gennaio 2027, ore 23:59 | Consegna finale su Moodle (−1 punto/giorno di ritardo) |

Le consegne avvengono **esclusivamente tramite Moodle**; non sono ammesse consegne via e-mail, così come richieste di feedback fuori dalle sessioni in classe.

---

## 📊 Valutazione

Punteggio massimo: **30 punti**, pari a **1/3 del voto finale del corso**. Criteri: correttezza scientifico-metodologica, inquadramento bibliografico, chiarezza e struttura della relazione, qualità grafica e cartografica, capacità di analisi critica, originalità e corretta citazione delle fonti, rispetto di tempistiche e istruzioni.

Il testo completo dei criteri e delle condizioni (proprietà intellettuale, divieto di collaborazione tra gruppi, uso consentito di strumenti IA) è nel Capitolato Tecnico.

---

## ⚖️ Licenza

Il materiale è distribuito con **licenza MIT** (vedi `LICENSE`). L'uso dei dati e dei materiali forniti è comunque regolato anche dalle condizioni specifiche indicate nel Capitolato Tecnico, che ne riserva l'uso a finalità didattiche nell'ambito del corso.

---

## 👤 Autore

**Alessio Rovere** — Università Ca' Foscari Venezia, Dipartimento di Scienze Ambientali, Informatica e Statistica.
