
---
layout: post
title: Pgenerosa_TagSeq_WGCNa_Results
date: '2021-03-18'
categories: Analysis
tags: pgenerosa, tagseq, WGCNA, RNAseq, gene expression, oxidative stress, hormetic priming
---


## First a review of our phenotype and experimental design...

- **Experimental design review** Here is our deisgn - circles represent samples that were sequenced using TagSeq (142 total samples)
	- Day 0 == after the initial priming period (primary exposure; 110 days) 
	- Day 7 == after the second exposure period (7 days) 
	- Day 14 == after the ambient recovery period (7 days) 
	- Day 21 == after the third expoosure (7 days) and the end of the experiment 

![Repeat_exposure_TagSeq](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Repeat_exposure_TagSeq.jpg "Repeat_exposure_TagSeq")

- **Phenotype review**
	- 'Primed' phenotype at the end of the experiment (day 21; cumulatively as day 131) had 
	larger shell size, respiration rate, and tissue biomass. Further, the primed phenotype 
	had lower total antioxidant capacity relative the the controls (not primed to early-life stress) **depicted below**

![Pgen_phenotype](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Pgen_phenotype.jpg "Pgen_phenotype")

## Why explore gene expression networks?
To investigate patterns of expression attributed with this phenotype and gain insight on molecular 
mechansisms of envrionmental learning. Weighted gene co-expression network analysis will determine gene 'modules' 
of interest that are associated with different expression trajectories. This is especially useful 
in our experimental to view pattern in response to the repeated and cumulative stress treatements. 

**Below** are WGCNA results with goseq follow-up and pooints for disucssion and future measurements

# WGCNA Analysis 

## DAY 7 
**What do we see?** 

There are **three** modules showing significant treatment effects:

- **brown**:
	- *WGCNA* = sig positive correlation with ambient (control - no priming) relative to primed animals - as groups with second treatment we see AM > MS and AM > MA
	- *vst expression* = the weight of this primary effect is due to the *lower vst expression in MA and MS treatments*
	- *goseq* = 
		a. oxidative stress (glutathione peroxidase)
		a. methanionine cycle activity and methyl group transfer (methanionine adenosyltransferase activity, SAM-dependent activity)
		a. fatty acid metabolism (acetyl CoA oxidase activity, lipid binding, lipid transporter activity) 
- **green**:
	- *WGCNA* = no sig effect of the primary treatment - as groups with secondary, we see AS > MM
	- *vst expression* = genes in this module show highest expression in the AS treatment - those not primed and initially exposed to acute *severe treatment (7 days)* 
	- *goseq* =
		a. ferric iron binding - (FeII activity)
- **yellow**
	- *WGCNA* = sig positive correlation with the primed animals relative control - as groups with second treatment we see a treament effect of the AS treatment
	- *vst expression* = genes in this modeule show lowers expression in the AS treament - however the main treatment effect is also evident with primed > control
	- *goseq* =
		a. housekeeping activity (ion exchange, DNA binding, transcription factor activity, signaling such as MAPK and phosphotyrosine residue binding)

![Day7_WGCNA](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Day7_WGCNA.jpg "Day7_WGCNA")


## DAY 14 
**What do we see?** 

There are **four** modules showing significant treatment effects:

- **brown**:

	- *WGCNA* = sig positive correlation with ambient (control - no priming) relative to primed animals - as groups we see a effect involving the AM treatment

	- *vst expression* = the weight of this primary effect is due to the *higher vst expression AM treatment*

	- *goseq* = 

		- oxidative stress (glutathione peroxidase, glutathione transferase activity)

		- methanionine cycle activity and methyl group transfer (methanionine adenosyltransferase activity, )

		- fatty acid metabolism (acetyl CoA oxidase activity, lipid binding, lipid transporter activity) 

		- proton gradient control (possibly due to hypercapnia?) - proton transmembrane transporter activity

		- others to look into are... endopeptidase activity, and carbonyl reductase and dehydrogenase activity

- **black + pink (clustered)**:

	- *WGCNA* = black has a significant primary treatment effect with higher expression in the moderate history - as groups we see both black and pink modules have an effect in the MS treatment

	- *vst expression* = genes in this module show highest expression in the MS treatment - those  primed and secondarily exposed to acute *moderate treatment (7 days)* - furtehr the weight of the primary treatment effect in the black module seems driven by this upregulation trend in the MS treatment

	- *goseq* =

		- oxidative stress - superoxide dismutase activity 

		- ion exchange / binding

		- complex I activity - NADH dehydrogenase 

- **magenta**
	
	- *WGCNA* = opposing effect of the black and pink module - 
	
	- *vst expression* = genes in this modeule show lowers expression in the MS treament 
	
	- *goseq* =
		
		- housekeeping activity (DNA binding, transcription factor activity, translation, etc.)


![Day14_WGCNA](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Day14_WGCNA.jpg "Day14_WGCNA")

## DAY 21 
**What do we see?** 

There are **six** modules showing significant treatment effects:
We will focus on **three of the six that show primar treatment effects**

- **magenta + blue (clustered)**:

	- *WGCNA* = Both have a significant effect of the primary treatment with higher expression in the ambient (control) history relative to the primed animals; when grouped, we see the main differences are in the treatment grops of ASM and ASA 

	- *vst expression* = genes in both modules hwo higher expression in the ASM group and blue includes also the ASA group 

	- *goseq* =
	
		- housekeeping, regulation of cell growth and differentiation - GTPase, DNA binding,RNA polymerase, spermadine synthase 

		- iron activity - ferric iron binding - carrier proteins invovled in metabolism and immune response; also possible are *ferric iron dependent demethylases such as TET and Jmj-C*

- **yellow**:

	- *WGCNA* = Both have a significant effect of the primary treatment with higher expression in  primed history relative to the control; the weight of this difference does not show a specific treatment group at Day 21 (solely main primary effect) 

	- *vst expression* = genes in this module have higher expression in the mdoerate 'primed' history than the control

	- *goseq* =
		
		- housekeeping - regulatory proteins ubiquitin, DNA binding, phospholipid binding, GTPase etc. 


![Day21_WGCNA](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Day21_WGCNA.jpg "Day21_WGCNA")
