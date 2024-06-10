# Planning for Survivorship measurements 

**This post is in progress, I am actively writing this post - check back soon for full content!**  


Experimental design and project planning notes for lifestage carry over project survival analysis.  

## Question of interest and hypothesis

*Does stress hardening increase temperature tolerance in oysters and does this effect vary by lifestage?*   

- **Hypothesis 1**: Stress hardening will increase survival times at elevated temperatures. 
- **Hypothesis 2**: The magnitude of sress hardening effects will vary by lifestage (i.e., between adults, seed, and spat). 

## General approach

Measure survival of individuals at high and control temperatures for oysters that were hardened and those that were not.  

## Overview of survivorship curve approaches 

There are three general statistical approaches that I am going to look into: Kaplan Meier, Cox proportional hazards, and logisitc regression.  

### Kaplan Meier approach

[A practical guide to understanding Kaplan-Meier curves (Rich et al. 2014)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3932959/):  

- Kaplan-Meier curves help us deal with missing observations in survival analyses. This can also be used when there are no missing observations to estimate survival and calculate survivorship metrics. 
- Time-to-event measurements including the Kaplan-Meier are used when there is a beginning and end point for all subjects within the course of the study (i.e., all subjects are alive at the start and are measured at the end of the study). 
- Subject is characterized by three variables: 1) time (serial time during study, i.e. no. of days), 2) their status at the end of the serial time - censored or event occurred, and 3) the study group they are in. 
	- For example, at the end of the study, a subject may be given a status of 1, meaning that the event (e.g., "mortality") occurred or a status of 0, meaning that the event did not occur and that individual was measured (i.e., censored and stayed alive).  
	- All individuals will therefore have a value of 0 at the beginning of the study, and could either have a value of 1 or 0 at each subsequent time point. 
	- "Censoring means the total survival time for that subject cannot be accurately determined. This can happen when something negative for the study occurs, such as the subject drops out, is lost to follow-up, or required data is not available or, conversely, something good happens, such as the study ends before the subject had the event of interest occur, i.e., they survived at least until the end of the study, but there is no knowledge of what happened thereafter."
- The interval is the time duration of known survival - this is terminated by mortality or the event of interest. Known survival can only be determined by the occurrance of the mortality event. Censored subjects are indicated as tick marks in the interval - they do not terminate the interval because the event has not yet occurrred/the subject is still alive. 
- For our use, since all oysters will be measured during the entire study, 1 indicates the event (mortality occurred) and 0 indicates the event did not occur (alive). 
- Further statistical tests can be analyzed using log rank tests or hazard ratios.  

[Understanding survival analysis: Kaplan-Meier estimate (Goel et al. 2010)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3059453/): 

- KM method involves computing probabilities of occurrence of the event at a point in time and multiplying these successive probabilities by any earlier probabilities to get a final survivorship estimate. 
	- Calculated as (number of subjects living at the start - number of subjects died) / (number of subjects living at the start)
	- Subjects who have died, dropped out, or moved are not counted as "at risk" - subjects censored do not count in the denominator. 
	- Log rank tests compare the groups statistically after generating curves.  

**Take home: KM curves are useful to incorporate censoring and are non-parametric. I need to determine whether this is the most powerful statistical tool we can use, given that we will not need to incorporate censoring in our study (we will measure every individual across the study).**  

### Cox proportional hazards model

The Cox model is semi-parametric, meaning that  

### Logistic regressions

This can overcome a limitation of the Cox model when time is in discrete categories, which generates a large number of ties. This could happen because we will monitor survival in 4-6 hour intervals. 


logistic mixed effect binomial regression (fusion paper) 


## Proposed experimental design 

xxx

Water changes how often? 
Jars of water at temperature ready  
Filtered water?  
Size of container?  
Temperature treatment level?  
Logger deployment  
Record animal length, width, depth 
Record survival every 2-6 hours? 
Definition of survival 
Reciprocal design


## Replication 

*Reciprocal exposure?* 

Adults: n=15 animals per treatment per family; n=3 families

- n=45 animals treated; n=45 animals control 
- n=7-8 animals control-high
- n=7-8 animals treated-high
- n=7-8 animals control-control
- n=7-8 animals treated-control

*Is this enough?* 

Seed: n=18 animals per treatment

- n=18 animals treated; n=18 animals control
- n=9 animals control-high
- n=9 animals treated-high
- n=9 animals control-control
- n=9 animals treated-control

*Is this enough?* 

Spat: Hundreds per treatment available 

- n=50-100 animals control-high
- n=50-100 animals treated-high
- n=50-100 animals control-control
- n=50-100 animals treated-control


## Data recording 

Spreadsheet
Animal ID's
Method of recording 
Temperature recording 
Time checked 

What is mortality? 

## Equipment required 

- Incubator
- Jars for adults 
- 24-well plates for spat; 6- well plates for seed 

## Next steps 

xxx