# Semio2Brain-Database [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4473240.svg)](https://doi.org/10.5281/zenodo.4473240)
Descriptive Seizure Semiologies and their multi-one-hot encoded categorical hierarchical brain localisations (11230 datapoints) and lateralisations (2391 datapoints) from 4643 patients across 309 included articles, as a Microsoft Excel Spreadsheet.

# Citing
If you use this database please cite the original paper describing the database and localisation results:
**Ali Alim-Marvasti, Gloria Romagnoli, Karan Dahele, Hadi Modarres, Fernando Pérez-García2, Rachel Sparks, Sebastien Ourselin, Matthew J Clarkson, Fahmida Chowdhury, Beate Diehl, John S Duncan. Probabilistic Landscape of Seizure Semiology Localising Values. Brain Communications. 2022 (In Press)**

## Seizure semiology
The initial or most prominently reported semiology (ipS) of patients with epilepsy were documented, firstly using the descriptions as reported (e.g., “right arm flexed and left arm extended”), and subsequently using summary terms at the point of data collection (e.g., “L asymmetric tonic”).

## Lateralising datapoints
Right vs left is can be meaningless without determining the laterality of the semiology and/or the patients’ dominant hemisphere. We collected laterality datapoints relative to the semiology as ipsilateral and contralateral; or dominant vs non-dominant hemisphere. Datapoint inputs to Semio2Brain database were at the level of individual patient-semiologies, such that if a right-sided semiology localised to the left, a “1” was inserted into the contralateral category. 

## Localising datapoints
Hierarchical top level localising categories, mainly lobar, were devised, these were temporal, frontal, parietal, occipital, cingulate, insula, hypothalamic, subcallosal, cerebellar with separate standalone (non-hierarchical) categories for sulci and interlobar junctions: frontotemporal, temporooccipital, temporoparietal, fronto-temporo-parietal, temporo-parieto-occipital, parietooccipital, frontoparietal and perisylvian. The hierarchy of brain regions was iteratively developed from the top-level regions-of-interest (ROI), in total 103 ROI categories. Each localising semiology from a patient resulted in a “1” being inserted into the relevant category. If a semiology localised to multiple categories, each received the full single datapoint. 

## Ground Truths (GT)
Only semiology from patients with the following ground truths about their lateralisation or localisation were collected: 
i) had epilepsy surgery and remained seizure-free for at least 12 months (Engel Ia or Ib, or ILAE 1 or 2, or Engel I if not otherwise specified, but not worse than Engel Ib or ILAE 2) – SF or EZ GT; 
ii) concordant imaging and electrophysiology, mostly MRI and EEG, but also PET or SPECT and EEG or MEG. 
iii) invasive stereotactic-EEG (SEEG) and/or cortical electrical stimulation (CS)

## Topological Prior Studies (TS)
In order to evaluate and mitigate the expected publication bias favouring TLE, we collected Boolean information on whether a reported semiology originated from a study which preselected patients based on pre-specified brain regions. For example, a report stating “we looked at patients with TLE…” would be labelled as a study with a pre-determined epileptic topological prior (ET), whereas, “we looked at 20 consecutive patients’ semiologies…” would be labelled as “spontaneous semiology (SS)”. CS studies were considered a method of preselection as they assessed the semiology-generating potential of pre-specified cortical regions. That is, we developed a Bayesian filter for datapoints from studies that preselected patients based on topological priors and when they did, we labelled these datapoints as topological studies (TS=ET+CS), and when they didn’t when labelled them SS.

# Funding
Wellcome/EPSRC Centre for Interventional and Surgical Sciences (WEISS) (203145Z/16/Z) to AAM.
