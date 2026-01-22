# dataset-affective-music-BCI

**Dataset: A closed-loop, music-based brain-computer interface for emotion mediation**

This repository contains the dataset accompanying the publication:

> **Ehrlich, S. K., Agres, K. R., Guan, C., & Cheng, G. (2019).**  
> *A closed-loop, music-based brain-computer interface for emotion mediation.*  
> **PLOS ONE, 14(3), e0213516.** https://doi.org/10.1371/journal.pone.0213516

The dataset is organized around **two experimental studies**:

- **Study I (listening):** music listening experiment (affective responses / ratings)
- **Study II (BCI):** closed-loop affective BCI experiment (EEG + adaptive music feedback)

Documentation for each study (protocol, data format, variables, etc.) is included in the respective study folders.

---

## Repository structure

```text
dataset-affective-music-BCI/
├── study I (listening)/
│   ├── data_all_participants.mat
├── study II (BCI)/
│   ├── P01      # EEG adn meta data of participant 1
│   ├── P02      # EEG adn meta data of participant 2
│   └── ...
├── study_I_documentation.pdf
├── study_II_documentation.pdf
└── README.md
```

---

## Study descriptions (brief)

### Study I – Listening experiment
**Purpose:** establish affective responses to music stimuli and collect ground truth labels for emotion-related targets.

**Design:** Participants listened to music excerpts and provided **self-report ratings** (e.g., arousal/valence-related measures).  
This study provides **behavioral affect annotations** and stimulus-related data that can be used for modeling affective responses to music.

**Folder:** `study I (listening)/`


### Study II – Closed-loop affective BCI experiment
**Purpose:** evaluate a **closed-loop affective BCI** that adapts algorithmic music generation based on the user’s brain state, aiming at emotion mediation.

**Design:** Participants interacted with a system that collected **EEG signals**, extracted affect-relevant information, and used this information to **adapt the music in real time** (neurofeedback loop).  
This study provides EEG recordings, event markers, system states, and additional behavioral measures depending on condition.

**Folder:** `study II (BCI)/`

---

## About the dataset

### Intended use
This dataset supports research in:
- affective computing and passive BCI
- music-induced emotion and music psychology
- neuroergonomics / human–AI interaction
- machine learning models for affect prediction and mediation

### Modalities and measures (overview)
Depending on the study, the dataset includes:
- **EEG recordings** (Study II)
- **music stimuli / musical parameters**
- **affect labels** from self-report ratings (Study I and/or Study II)
- **timestamps / event markers** for synchronized analysis

For exact data formats, EEG configuration, label definitions, and event descriptions, consult the documentation inside each folder.

---

## Citation

If you use this dataset in academic work, please cite:

```bibtex
@article{ehrlich2019closedloop,
  title   = {A closed-loop, music-based brain-computer interface for emotion mediation},
  author  = {Ehrlich, Stefan K. and Agres, Kat R. and Guan, Cuntai and Cheng, Gernot},
  journal = {PLOS ONE},
  volume  = {14},
  number  = {3},
  pages   = {e0213516},
  year    = {2019},
  doi     = {10.1371/journal.pone.0213516}
}

