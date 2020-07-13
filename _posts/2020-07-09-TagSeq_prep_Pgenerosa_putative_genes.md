---
layout: post
title: TagSeq_prep_Pgenerosa_putative_genes
date: '2020-07-09'
categories: Summary, Preparation
tags: geoduck, proteins, tagseq, blast
---


## Summary

### Table: Results of the repeat pCO2 stress exposure experiment in 2019
##### stress acclimation improves performance and oxidative status under subsequent stress encounter(s)

 life stage  | age  | Stress acclimation (Y/N) | intensity (uatm)  | Repeat exposure (Y/N) | intensity (uatm) | Respiration rate | Shell growth | Tissue growth (AFDW) |Antioxidant capacity |
 --------: | --------: | --------: | --------: | --------: | --------:| --------: | --------: |  --------: | --------: |
postlarval 'settlement'; pediveliger to juvenile | 30 d to 5 mo post-fertilization  | N  | 900 µatm (ambient) |  N | 900 µatm (ambient)  | - | - | ↓''   | ↑''
|   | N  | 900 µatm (ambient) | Y  | 3000 and 4900 µatm (moderate & severe)  | ↓' |  ↓'' |  ↓'' | ↑''
  |   |  Y | 3000 µatm (moderate)| N  | 900 µatm (ambient)  | ↓'' | -  | ↑'' | ↓''
  |   |  Y | 3000 µatm (moderate)| Y  |3000 µatm (moderate) | ↑' | ↓'' | ↑'' | ↓''
  |   |  Y | 3000 µatm (moderate)| Y  | 3000 and 4900 µatm (moderate and severe) | ↑'' |  ↑'' | ↑'' | ↓''

> *↑ ↓ relative rates/analysis between treatments after a single repeat exposure (') and multiple exposures ('')*

----------------------------------------

## Moving forward...
#### Questions:

> *Note: the acclimated phenotype was had both greater shell size/tissue biomass/respiration rate and reduced antioxidant protein activity*

  - Can moderate oxidative stres or mitchondrial dysfunction improve performance?
  - Is there an alternative mitchondrial pathway in acclimatized phenotype to permit peroformance  and decrease ROS?
  -  Does the paternal envrionment increase mitchodrial flexibility in progeny under equal or greater stress intensity?
    - driven by non-genetic inheritance?


----------------------------------------
## Objective:

  - investigate mitchondrial mechanism(s) driving the differential phenotype
  - ~4 samples from two treatments in the experiment above

### Mechanism Figure:


![Mechanism](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/2020_AOX_RET_Crosstalk.JPG "Mechanism")

>   #### Current findings
  - *Acclimated phenotype* : = ↑ growth, ↑ metabolic rate, ↓ CSR
  - *Not acclimated* = ↓ growth, ↓ metabolic rate, ↑ CSR


>   #### Next Analysis
  - *Acclimated phenotype* : proposed pathway =  Alternate oxidase (AOX)
  - *Not acclimated* :  proposed pathway =  Reverese electron transport (RET)
  - **TagSeq & metabolomics** : investigate a stress-acclimation-dependent effect on mitchondrial function(s) [targets: AOX, UCPs, sirtuins, complexes 1 & III, ATP, NAD+:NADH, CoQ:CoQH]

>   #### Future directions
  - Mitonuclear crosstalk :
    - *What is the role of stress hormesis (via ocean acidification exposure(s)) on DNA/histone methylation (i.e. Jmj-C and TET activity) and anterograde and retrograde signaling (i.e. unfolded protein response)?* *Is there as stress timing- (i.e. paternal & early-life environment) and intensity-dependent (i.e. duration, magnitude, frequency) effect?*

----------------------------------------

### I) TagSeq
#### Identified target genes of interest (GOIs)

### 1. AOX

*putative P. generosa seqID:* **PGEN_.00g108770**

> ##### Why alternate oxidase (AOX)?
  - Function: catalyzes the oxidation of ubiquinol and reduction of oxygen to water. Protons taken from uqiquinolnot the mitchondrial matrix (unlike the cytochrome c oxidase reaction; complex IV).
  - Not inhibited by cyanide (unlike complex IV) - allows cyanide-resistance OXPHOS
  - Altogether, allows ATP production and reduces ROS under envrionmental disturbances.
  -  AOX is previously thought to be limited to plants, fungi and protists but has    recently expanded to a variety of animalia taxa
  - AOX is theorized to be prevalent in animals that have frequent transitions from hypoxia to reoxygenation during thier life history. AOX s likley help these taxa survive transitions from anaerobic conditions without substantial damage cause to membrrane lipids and proteins by ROS (McDonald and Gospodaryov 2019).
  - In Eastern oyster, Crassostrea virginica, there are two splice forms of AOX mRNA which are expressed in a number of tissues (Liu and Guo, 2017) and assist resitance to hypoxia-reoxygenation

> ##### What is mitchondrial dysfunction?
  - Mitochondrial dysfunction is defined as electron leak or increase of ROS production due to an alteration of normal electron transport.
  - Causes:
    - Reverese electron transport (RET): can occur under (i) high pools of reduced metabolites NADH:NAD+ and CoQH:CoQ; well-chracterized under dietary restriction (ii)  pH gradient ([H+]) and/or protonmotive force of the inner mitchondrial membrane

> ##### In summary...
  - AOX is an alterantive mitchondrial pathway known as an adaptive response in bivalve taxa under envrionmnental stress. Thus, the lower antioxidant response and greater performance of the stress-accliamted phenotype in 2019 (table above) eludes to higher ATP and lower ROS -- this may be driven by enhanced mitchondrial flexibility (i.e. via AOX) due to prior stress priming!

### 2. SIR2

*putative P. generosa seqID:* **PGEN_.00g048200**

> ##### About:
  - sirtuins are NAD+ dehydrogenases
  - deacetylation of proteins can increase proteostasis and alleviate dysfunction - i.e. sirtuins can increase the antioxidant response

### 3. Mitchondrial carrier protein

*putative P. generosa seqID:* **PGEN_.00g063670**

> ##### About:
  - uncoupling proteins are activated by lipid peroxidation - thus they are a response of oxidative stress and are increased during dysfunction
  - uncoupling proteins reduce the protonmotive force (and pH gradient) of the inner mitchondrial membrane reducing ROS production from mitchondrial dysfunction at the expense of reduced potential for ATP

### 4. NADH dehydrogenase

*putative P. generosa seqID:* **PGEN_.00g299160**

> ##### About:
  - complex 1 of mitochondrial electron transport chain.
  - major source of mithcondrial ROS production and increases activity under dysfunction

### 5. Cytochrome c reductase

*putative P. generosa seqID:* **PGEN_00g275780**

> ##### About:
  - complex III of mitochonrial electron transport chain
  - major source of mithcondrial ROS production; may reduce abundance/activity under mitchondrial dysfunction - Example: high ratio complexI:complexIII is an indicator of reverese electron transport

### 6. Jumonji C and Ten-eleven translocation

*putative P. generosa seqID:* **PGEN_.00g257110** (Jumonji-C)

> ##### About:
  - Jumonji-C and TET function in the demethylation of histones and DNA, respectively - a post-translational (histones) and DNA modification that effects transcriptional regulation
  - Why is this interesting in response to OA stress?
    - Jumonji-C and TET activity is dependent on Fe2+. Chelated Fe2+ is released during intracellular acidosis - further Fe2+ is reduced to Fe3+ from the Fenton reaction also catalyzed by acidosis.
  - Altogether, an iron-acidosis interaction may have downstream effects on non-genetic transcriptional regulation - this is an interesting direction to investigate the role of epigentics in mitonucluear crosstalk and hormetic conditioning under OA conditions!

### II) Metabolomics

#### 1. ADP/ATP

  > - Expected ATP: **AOX pathway >** RET/dysfunction pathway

#### 2. NAD+:NADH

> - Expected NAD+/NADH: AOX pathway **< RET/dysfunction pathway**
> - Note: although dysfunction can be casued by a high pool of NADH, the high activity of complex I oxidizes NADH to NAD+.

#### 3. CoQH

> - Expected CoQH: AOX pathway **< RET/dysfunction pathway**

----------------------------------------

## Resources:
#### Panopea generosa (Pacific geoduck) draft genome
- link: http://dx.doi.org/10.17605/OSF.IO/YEM8N

#### Repository of target genes
 > *note*: repo originally in preparation for qPCR - contains blast hits and primer3 outputs for several target GOIs and normalization genes

- link: https://github.com/SamGurr/Pgenerosa_primers
