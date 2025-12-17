# Bert-Driven-Equalizer

A **semantic EQ**: turn natural language descriptors into automatic equalization curves.  
This project is part of an in-progress Master’s thesis exploring **BERT contextual embeddings + regression → 40-band EQ curves**.

---

## Quick Overview

Describe how you want the sound to change (e.g., *warm*, *bright*, *muddy*), and the model predicts a full **40-band ERB EQ curve** to match that descriptor.  
You can run it with the provided notebooks and preview results in this repo.

---

## Files

- **Notebooks**  
  - `Play_and_Listen.ipynb` – quick demo + interactive inference  
  - `ModelTraining&Testing.ipynb` – train / evaluate  
  - `Embedding-extraction.ipynb` – BERT embedding extraction  
  - `data-preprocess.ipynb` – data setup (SocialEQ dataset)

- **Models**  
  - `BERT_*Fold_MAE.keras` – saved checkpoints

- **Results/** – figures from the experiments  
- **App/** – prototype application UI & screenshots  
- `e_gtr_short.wav` – sample audio

---

## Run It

1. Open **Play_and_Listen.ipynb**
2. Load a model checkpoint (e.g., Fold 4)
3. Enter a descriptor (text)
4. Hear the equalized audio

---

## Results

Below are the key **Results** showing model performance and example predictions.

### MAE & PCM Results vs Baseline

*Mean Absolute Error per band across folds*

![MAE](results/MAE_Comparasons.png)

*Partial Curve Mapping distance across folds*

![PCM](results/PCM_Comparasons.png)

---


> These figures show how predicted 40-band curves align with human curves.
![curves1](results/semantic_plots_page_1.pdf)
---

## Application (Prototype)

This folder contains a **real-time EQ + source separation prototype**.  
Users can type a descriptor and apply semantic EQ to audio/video playback.

### App UI Screenshots

#### Main View
![App Main](App/app_main.png)

#### Descriptor Input & Curve Preview
![Input & Curve](App/app_input_curve.png)

#### Stem Controls
![Stems UI](App/app_stems.png)

---

## Notes

- Works with **SocialEQ dataset**.  You can get the SocialEQ dataset from [here](https://www.dropbox.com/scl/fo/ulk8t7ad5b1js8qwuph3f/ANnatQNiD1QoQoeDDZktHjM/data/raw?e=1&preview=eq_contributions.csv&rlkey=we20hw9qu94wytocopw5np1yj&subfolder_nav_tracking=1&dl=0).
- The EQ output is a **40-band curve** suitable for further DSP.

---
