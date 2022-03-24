---
layout: post
title: Oyster hemolymph flow cytometry
date: '2022-03-24'
categories: Processing, Analysis
tags: crassostrea, oyster, OA, hemolymph, flow cytometry, C6 plus, BD biosciences
---

# Flow Cytometry for Oyster (*Crassostrea virginica*) Hemolymph 
Last Revised: 20220324 SJ Gurr


## <a name="About experiment"></a> **About experiment**:
---------
(insert link to the google drive presentation)


#### Goals:





#### About probes of interest:

- add here...
- add here...
- add here...
- add here...

#### SOPs:  

(insert link(s) to our master google drive SOP(s))

C6 Plus manual (BD Biosciences; link here <https://www.bdbiosciences.com/content/dam/bdb/marketing-documents/BD-Accuri-C6-Plus-Users-Guide.pdf>)


#### Experimental design/timeline 

(insert photos of the trial) 

* chemistry

- note: the mass flow controller for the 'high' treatment was bumped to 7.0, good to note for future efforts but is merely a snapshot due top the temperature, season, ambient conditions, etc. 

| Carbonate chem  |      pCO2 (uatm)      |       pH      |        add here...       |    add here...         | 
| -----------     | -----------  | ----------- |  -----------  | ----------- |  
| Low             |    add here... |   add here...   | add here...     |   add here...    |        
| High            |    add here...    |    add here... |    add here...   |    add here...   |         
  


## <a name="Analysis of flow cytometry data"></a> **Analysis of flow cytometry data**:
---------
|  Steps | Flow Cy Probes |
|----|-----|
|  I | SYBR Green + potassium iodide |
|  II | add here... |
| III  | add here... |
| IV  | add here...  |



**Figure of flourochromes** from the C6 Plus manual (BD Biosciences; like above in 'SOPs')

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_BD_Manual_FL_wavelengths.PNG "Flow_cy_BD_Manual_FL_wavelengths")

## I.) SYBR Green + potassium iodide 


### I.A.) Initial look with SSC vc FSC

* forward scatter and side scatter with SYBR green is an ideal first step when analyzing hemolymph quality and initial gating of your template - these paremeters represent the size of the particles (forward scatter) and their complexity (side scatter) 

	- *NOTE! the initial scatterplot view of your flow cytometry data (assuming no threshold(s) set) will be a messy cloud of noise.* 

* zoom into the tail end of the x axis (in this case forward scatter 'FSC-H') and you should see an upward curl of the data in the y axis. This is the region of your hemocytes around 10^5.8 - 10^6.7 on forward scatter log scale


*Figure below*: raw data on side and forward scatter *ignore the color-coded regions as this will initially be all one color at this stage*

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_sscfsc_raw.PNG "Flow_cy_sscfsc_raw")


### I.B.) gate with FL1 

* SYBR green binds to DNA and flouresces in the FL1 (533/30) between 10^6 and 10^7

* create a gate calling the distinct peak wihtin this region

*Figure below*: SYBR green + potassium iodide after 1 hr 14 minute incubation of oyster hemocytes. Gated region titled 'FL1'_Allhem'. *ignore the color-coded regions as this will initially be all one color at this stage*

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_FL1_SYBR_green.PNG "Flow_cy_FL1_SYBR_green")


### I.C.) Overlay FL1 gate to SSC vc FSC, gate cell types

* view your SSC vc FSC **for all your individuals** overlaid with the gated FL1 region, you should now see distinct 'clouds' or groupings of datapoints. These are **all cells with fouresced DNA (from FL1)** and you can now determine cell types!

	- *NOTE! review your species of interest as taxa differ in the number of parsable hemocyte types* 

*Figure below*: SSC vc FSC plot gated for the FL1 - four new gates created and color coded for cell types:

- <span style="color:pink">IG</span> = immanture granolocytes
	
- <span style="color:purple">MG</span> = mature 
	
- <span style="color:orange">MA</span> = mature granulocytes
	
- <span style="color:yellowgreen">Degran</span> = degranulated cells
	
- <span style="color:red">All</span> = all hemocytes, gated around the entire area after the four cell types/regations were determines

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_sscfsc_gated.PNG "Flow_cy_sscfsc_gated")


### I.D.) Live vs. dead using FL3 

* call the live and dead regions in FL3 - PerCP-H 

## II.) DCFH-DA

DCFH-DA

some notes...
* remove the gate for the FL1 that was made with the SYBR green
* diffueses into cell - hydrolyzes trapped in cell -  then oxidizes to DCF by oxided to DCF by ROS and then flouresces 
* geometric mean - calculated population flourescence? 
* do we want to normalize by live cells within sample/cell type 
* mean flourescence intensity - what does this mean? An arbitrary unit? flourecence intensity increases logarithmically - mean is skeweed accurate cannot be estimated due to log scale - geometric mean is teh fourescence intensity of the population 



Figure dump... drag and drop to above where needed as you edit..

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_Beads_mature_granulocytes_gates.PNG "Pgen_histology_figs")

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_DCFHDA_parsed_FL1.PNG "Pgen_histology_figs")

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_gate_FL1__for_DCFHDA.PNG "Pgen_histology_figs")

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_gated_OFF_DCFHFDA.PNG "Pgen_histology_figs")

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_interection_live_cells_by_type.PNG "Pgen_histology_figs")

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_matrue_granulocytes_Beads.PNG "Pgen_histology_figs")

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_sscfsc_gated.PNG "Flow_cy_sscfsc_gated")

![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_SYBRGreen_PI_master_gated.PNG "Flow_cy_SYBRGreen_PI_master_gated")


![Figure](https://samgurr.github.io/SamJGurr_Lab_Notebook/images/Flow_cy_FL1_SYBR_green.PNG "Flow_cy_FL1_SYBR_green")
