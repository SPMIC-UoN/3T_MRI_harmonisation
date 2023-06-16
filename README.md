# README

This repository contains code and data associated with the manuscript "A resource for development and comparison of multi-modal brain 3T MRI harmonisation approaches".

## Code

Code (jupyter notebooks) used to generate manuscript figures are available under "scripts"

## Data

We provide IDP and IQM text files containing all data necessary to generate manuscript figures under "data".

In addition, we provide a summary IDP CSV file containing all baseline IDPs and IQMs (i.e. excluding denoised IDPs).

idp_vis.ipynb - the main script for quantifying and comparing IQMs and IDPs
combat.ipynb - used to compare IDPs harmonised using implicit harmonisation tools (combat, covbat)
denoise.ipynb - used to compare denoised dMRI data IDPs to raw dMRI data IDPs
first_vs_mist.ipynb - used to compare unimodal and multimodal subcortical segmentations
freesurfer_fastsurfer.ipynb - used to compare atlas-based, Freesurfer and FastSurfer cortical parcellations



## Details related to access to the raw data (following BIDS convention)

- [ ] Citation:

When using this dataset, please cite the following Warrington, Ntata et al. "A resource for development and comparison of multi-modal brain 3T MRI harmonisation approaches", bioRxiv



## Overview

- [ ] Project name: A resource for development and comparison of multi-modal brain 3T MRI harmonisation approaches

- [ ] Years that the project ran: 2018-2021

- [ ] Description of the contents of the dataset: ten participants, six 3T scanners across five sites and three major vendors, within-participant within-scanner and between-scanner repeats, five modalities.

## Methods

### Subjects

N = 10 healthy participants (mean age 34 ± 9.4 years; 8 male, 2 female)

Subject     Sessions
03286       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001
03997       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001
10975       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001
12813       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001
13192       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF1PRI002 OXF1PRI003 OXF1PRI004 OXF1PRI005 OXF1PRI006 OXF2PRI001 OXF3TRI001
13305       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001
14221       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001
14229       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF2PRI002 OXF2PRI003 OXF2PRI004 OXF2PRI005 OXF2PRI006 OXF3TRI001
14230       NOT1ACH001 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001 OXF3TRI002 OXF3TRI003 OXF3TRI004 OXF3TRI005 OXF3TRI006
14482       NOT1ACH001 NOT1ACH002 NOT1ACH003 NOT1ACH004 NOT1ACH005 NOT1ACH006 NOT2ING001 NOT3GEM001 OXF1PRI001 OXF2PRI001 OXF3TRI001

### Apparatus

Scanners:
1. Philips Achieva, 2. Philips Ingenia, 3. GE MR750, 4. Siemens Prisma (32ch), 5. Siemens Prisma (64 ch), 6. Siemens Trio

Modalities:
1. T1w, 2. T2w FLAIR, 3. diffusion MRI (dMRI), 4. resting-state functional MRI (rsfMRI), 5. susceptibility-weighted imaging (SWI)


### Experimental location

Scanners are located across five sites in the United Kingdom.

3T GE MR750: SPMIC-QMC, Nottingham
3T Philips Achieva: SPMIC, Nottingham
3T Philips Ingenia: SPMIC, Nottingham
3T Siemens Trio: WIN-FMRIB, John Radcliffe Hospital, Oxford
3T Siemens Prisma: WIN-OHBA, Warnefor Hospital, Oxford
3T Siemens Prisma: OCMR, John Radcliffe Hospital, Oxford

SPMIC - Sir Peter Mansfield Imaging Centre
SPMIC-QMC - SPMIC-Queen's Medical Centre
FMRIB - Oxford Centre for Functional MRI of the Brain
OHBA - Oxford Centre for Human Brain Activity
OCMR - Oxford Centre for Clinical Magnetic Resonance Research

### Notes
Anatomical data have been defaced following the UKBB defacing procedure. Defacing masks are available in each session directory as sub-<subID>_ses-<sesID>_mod-T1w_defacemask.nii.gz.

At time of release, SWI data were not yet incorporated in to the BIDS standard. The SWI extension proposal (https://bids-specification.readthedocs.io/en/v1.2.1/06-extensions.html: accessed Autumn 2022) was used to define SWI data structure.
