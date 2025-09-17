
# Cognitive Science Course Projects

This repository documents my journey through four major neuroscience and cognitive science projects, each tackling a unique aspect of perception, neural coding, or brain imaging. Here’s a more personal overview of what I did in each project:

---

## HW1: Psychophysical Analysis of Face Perception

In the first project, I set out to understand how people perceive and recognize faces, especially when those faces are morphed between two identities. During Phase 1, I focused on quantifying perceptual sensitivity—how well participants could tell two faces apart under different visual conditions. I used psychometric curve fitting and ROC analysis to get at the heart of this sensitivity, and then dug deeper to see how it changed with different image filtering and even with participant age. The statistical tests (Friedman, Wilcoxon) helped me test my hypotheses and validate the findings.

Phase 2 was all about hands-on experimentation. I designed a PsychoPy experiment where participants judged morphed faces, with images carefully selected from morph continua. Each trial asked them to decide which identity the image resembled more. After collecting responses, I fitted psychometric curves and estimated the Just Noticeable Difference (JND) for each feature, revealing how finely people could discriminate between faces depending on the transformation.

---

## HW2: Single-Cell Analysis and Neural Coding

This project started with building a spike-sorting pipeline for single-channel extracellular recordings. I filtered the data, detected spikes, and used PCA and clustering to sort them, always checking my results against ground-truth spike times. The second part of Phase 1 took me into the world of IT cortex recordings, where I analyzed responses from 92 neurons across thousands of trials and hundreds of images. I used peri-stimulus time histograms, Fano-factor analysis, mutual information, and d′ to explore how neurons responded to different categories, and constructed representational dissimilarity matrices to compare neural geometry to ground-truth categories. A GLM analysis showed that while IT activity reflects category structure, it does so only modestly at the population level.

In Phase 2, I replicated a closed-loop visual stimulus paradigm in macaque IT cortex. By analyzing firing rates from both evolution and auxiliary blocks, I was able to confirm a progressive increase in neural responsiveness in the main closed-loop sections. I also proposed alternative fitness criteria for future experiments, thinking about new ways to probe neuronal response properties.

---

## HW3: EEG Analysis of Visual Object Processing

For the third project, I investigated how the brain processes visual objects using EEG during a rapid serial visual presentation (RSVP) paradigm. Participants viewed images from two categories—faces and dollhouses—while I recorded EEG from 64 electrodes. The data went through a thorough preprocessing pipeline, including filtering, epoching, baseline correction, and ICA for artifact removal. I computed event-related potentials (ERPs) and used statistical tests to highlight differences between categories, especially at occipito-temporal electrodes.

I also performed time-frequency analysis to look at modulations in alpha, beta, and gamma bands, and used multivariate pattern analysis (MVPA) to quantify how well the EEG could distinguish between faces and dollhouses. To bridge brain activity with artificial neural networks, I constructed representational dissimilarity matrices from EEG and compared them with those from CORnet-S, a deep neural network model. Representational similarity analysis revealed that early EEG time windows matched lower layers of CORnet-S, while later windows aligned with higher-level layers, mirroring the hierarchy of the human ventral stream.

---

## HW4: fMRI Analysis of Visual Stimuli

The final project explored brain activation patterns in response to different visual stimuli using fMRI. I analyzed preprocessed data from a block design experiment, which included both localizer and extended runs. Using a general linear model (GLM) with the Glover hemodynamic response function, I computed contrasts to examine condition-specific and hemispheric differences. The results showed clear and significant activation differences between conditions, with robust bilateral activation for Conio vs Magnu and stronger activation for Magnu vs Cargo compared to Cargo vs Magnu. The z-scores confirmed the statistical significance of these findings, highlighting the brain’s nuanced response to different visual categories.
