# Cognitive Science Course Projects

This repository contains four major neuroscience and cognitive science projects, each exploring different aspects of perception, neural coding, and brain imaging. Below is an overview of each project and its phases.

---

## HW1: Psychophysical Analysis of Face Perception

### Phase 1: Sensitivity to Facial Identity
- Investigated human sensitivity to facial identity using morphs between face pairs.
- Explored perceptual sensitivity: how accurately participants distinguish identities under different visual conditions.
- Quantified sensitivity using:
  - Psychometric curve fitting (sigmoid function, β parameter).
  - ROC analysis (area under curve, sROC).
- Analyzed β across spatial frequency conditions (intact, low-pass, high-pass).
- Tested hypotheses with Friedman and Wilcoxon signed-rank tests.
- Explored the relationship between sensitivity and participant age.

### Phase 2: Psychophysical Experiment Design
- Designed and implemented a PsychoPy experiment to study perceptual sensitivity to morphed faces.
- Used morph continua between two identities, selecting 10 morph levels per continuum.
- Each image presented 10 times (400 trials total).
- Participants indicated which identity the image resembled more.
- Fitted psychometric (sigmoid) functions to responses, estimating Just Noticeable Difference (JND) for each feature.
- Results revealed discrimination ability under different shape and appearance transformations.

---

## HW2: Single-Cell Analysis and Neural Coding

### Phase 1: Spike Sorting and IT Cortex Analysis
- Developed a spike-sorting pipeline for single-channel extracellular recordings.
- Applied Butterworth band-pass filtering, spike detection, PCA, and k-means clustering.
- Assessed clustering performance against ground-truth spike times.
- Analyzed a large IT-cortex dataset (92 neurons, 5000 trials, 500 images, 4 categories).
- Used PSTH, Fano-factor, mutual information, and d′ to characterize category-selective responses.
- Constructed representational dissimilarity matrices (RDMs) and compared neural geometry to ground-truth categories.
- GLM analysis showed modest population-level category structure.

### Phase 2: Closed-Loop Visual Stimulus Paradigm
- Replicated a closed-loop stimulus paradigm in macaque IT cortex.
- Extracted firing rates from main (evolution) and auxiliary (natural image) blocks.
- Validated progressive increase in neural responsiveness in evolution blocks.
- Proposed alternative fitness criteria for future experiments.

---

## HW3: EEG Analysis of Visual Object Processing

- Investigated neural dynamics during a Rapid Serial Visual Presentation (RSVP) paradigm using EEG.
- Participants viewed images from two categories (faces, dollhouses); EEG recorded from 64 electrodes.
- Preprocessing: filtering, epoching, baseline correction, ICA artifact removal.
- Computed ERPs for both categories; statistical tests revealed significant differences at occipito-temporal electrodes.
- Time-frequency analysis showed category-related modulations in alpha, beta, gamma bands.
- Multivariate pattern analysis (MVPA) quantified discriminability; temporal and spatial MVPA revealed informative patterns.
- Constructed RDMs from EEG and compared with CORnet-S deep neural network layers using Representational Similarity Analysis (RSA).
- Found correspondence between EEG time windows and CORnet-S layers, paralleling human ventral stream hierarchy.

---

## HW4: fMRI Analysis of Visual Stimuli

- Investigated brain activation patterns in response to different visual stimuli (Conio, Magnu, Cargo) using fMRI.
- Analyzed preprocessed data from a block design experiment (localizer and extended runs).
- Applied GLM with Glover HRF and computed six contrasts for condition and hemispheric differences.
- Found significant activation differences between conditions:
  - Conio vs Magnu: robust bilateral activation.
  - Magnu vs Cargo: stronger activation than Cargo vs Magnu.
- Z-scores indicated strong statistical significance for condition-specific neural responses.
