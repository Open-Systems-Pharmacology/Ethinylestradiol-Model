The general workflow for building an adult PBPK model has been described by Kuepfer et al. ([Kuepfer 2016](#5-references)). Relevant information on the anthropometry (height, weight) was gathered from the respective clinical study, if reported. Information on physiological parameters (e.g. blood flows, organ volumes, hematocrit) in adults was gathered from the literature and has been incorporated in PK-Sim® as described previously ([Willmann 2007](#5-references)). The  applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available 'PK-Sim® Ontogeny Database Version 7.3' ([PK-Sim Ontogeny Database Version 7.3](#5-references)).

The following steps were undertaken in model development:

1. Define lipophilicity and distribution model on data after i.v. administration with linear total hepatic clearance fitted to data and renal clearance set to literature value ([Ezuruike 2018](#5-references)).

2. Predict p.o. data after single dose and at steady state 

3. Detail metabolic contribution of different CYPs and UGTs to total hepatic clearance.

Details about input data (physicochemical, *in vitro* and clinical) can be found in [Section 2.2](#2.2-data).

Details about the structural model and its parameters can be found in [Section 2.3](#2.3-model-parameters-and-assumptions).

A standard female subject was created based on the European (ICRP,2002) PK-Sim database (age = 30 y, weight = 60 kg, height = 163 cm, BMI = 22,58 kg/m2) and used for simulations, until stated otherwise. Expression of the enzymes CYP3A4, CYP2C9, CYP1A2, CYP2C8, and UGT1A1 from RT PCR database were added.
