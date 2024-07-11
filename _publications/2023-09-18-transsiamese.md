---
title: "TransSiamese: A Transformer-Based Siamese Network for Anomaly Detection in Time Series as Approach for Fault Location in Distribution Grids"
collection: publications
permalink: /publication/2023-09-18-transsiamese
excerpt: ''
date: 2023-09-18
venue: 'IEEE Access'
#slidesurl: 'http://academicpages.github.io/files/slides3.pdf'
paperurl: 'http://eliasherrero.es/files/TransSiamese_A_Transformer-Based_Siamese_Network_for_Anomaly_Detection_in_Time_Series_as_Approach_for_Fault_Location_in_Distribution_Grids.pdf'
citation: 'J. G. Fornás, E. H. Jaraba and A. L. Estopiñan, "TransSiamese: A Transformer-Based Siamese Network for Anomaly Detection in Time Series as Approach for Fault Location in Distribution Grids," in IEEE Access, vol. 11, pp. 103431-103451, 2023'
---

Fault localization in distribution grids represents a crucial aspect in achieving 
the concept of smart grids within electrical networks. 
Despite the existence of various approaches to address this issue, it remains an 
open and challenging topic in real situations and, therefore, complex grids.

![Alt text](/images/access-gagraphic-3316600.jpg "Connection diagram")

One of the main challenges stems from the scarcity of labelled real-world examples 
is due to the inherent chaotic nature of faults (short circuits between a phase and 
ground). Obtaining sufficient fault examples for neural network training purposes 
becomes extremely difficult. 

Efforts have been made to simulate fault signals and apply data augmentation 
techniques. However, for fault location specifically, classical augmentation 
techniques are not applicable due to the unique nature of the fault signals. 
In this paper, we propose a novel approach to address the problem of extracting 
fault location information from TDR (Time Domain Reflectometry) signals. This kind 
of signals, involve injecting pulses into the grid and record these pulses as a 
bounced signal due to the different impedance changes of the grid. 

Our approach relies on employing a Transformer for anomaly detection. 
This Transformer-based Siamese network architecture (abbreviated by TransSiamese) 
is inspired by TranAD model.This Transformer has been modified to be trained in a 
Siamese way with a few examples (pre-fault signals/normal state and fault 
signals/abnormal state). After training phase, we can run inference mode by 
feeding it signals representing faulty grid states (fault signals). The Transformer 
attempts to predict the evolution of the signal, however, from a certain point 
to the end, the predicted fault signal deviates from the True signal supplied.

![Alt text](/images/forna5-3316600-large.gif "TransSiamese")

Thanks to the intrinsic property of the Siamese network, it dampens the differences 
between the learned and the current signal when it comes to pre-fault; 
on the contrary, it enhances these differences when we are immersed in a fault signal.