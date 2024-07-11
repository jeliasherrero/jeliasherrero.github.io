---
title: "Detection and classification of fault types in distribution lines by applying contrastive learning to GAN encoded time-series of pulse reflectometry signals"
collection: publications
permalink: /publication/2022-01-GANencoded-TimeSeries
excerpt: ''
date: 2022, January
venue: 'IEEE Access'
#slidesurl: ''
paperurl: 'http://eliasherrero.es/files/Detection_and_Classification_of_Fault_Types_in_Distribution_Lines_by_Applying_Contrastive_Learning_to_GAN_Encoded_Time-Series_of_Pulse_Reflectometry_Signals.pdf'
citation: 'J. G. Fornás, E. H. Jaraba, A. L. Estopiñan and J. Saldana, "Detection and Classification of Fault Types in Distribution Lines by Applying Contrastive Learning to GAN Encoded Time-Series of Pulse Reflectometry Signals," in IEEE Access, vol. 10, pp. 110521-110536, 2022'
---

This study proposes a new method for detecting and classifying faults in distribution lines. The physical principle of classification is based on time-domain pulse reflectometry (TDR). These high-frequency pulses are injected into the line, propagate through all of its bifurcations, and are reflected back to the injection point. According to the impedances encountered along the way, these signals carry information regarding the state of the line. In the present work, an initial signal database was obtained using the TDR technique, simulating a real distribution line using (PSCAD™). By transforming these signals into images and reducing their dimensionality, these signals are processed using convolutional neural networks (CNN). In particular, in this study, contrastive learning in Siamese networks was used for the classification of different types of faults (ToF). In addition, to avoid the problem of overfitting owing to the scarcity of examples, generative adversarial neural networks (GAN) have been used to synthesise new examples, enlarging the initial database. The combination of Siamese neural networks and GAN allows the classification of this type of signal using only synthesised examples to train and validate and only the original examples to test the network. This solves the problem of the lack of original examples in this type of signal of natural phenomena which are difficult to obtain and simulate.

![Alt text](/images/Methodology.png "Structure")
