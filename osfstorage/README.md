# Open Access: The Effect of Neurorehabilitation on Multiple Sclerosis – Unlocking the Resting-State fMRI Data

Crawled from [OSF](https://osf.io/p2kj7/)

## Description

We publish fMRI data of 60 people with Multiple Sclerosis before and after two months of neuroproprioceptive "facilitation and inhibition" treatment. 

**For more details on the original study design as well as the acquisition parameters, please consult our [Data Report][1]**

The data contain the following information:

----------
**clinical.csv**
 
 Clinical information about subjects. 
 
 - **ID**: subject identifier. 
 - **SEX**: "M" or "F" identifying males and females.
 - **MS_TYPE**: type of multiple sclerosis either "remitting_relapsing", "primary_progressive" or "secondary progressive".
 - **AGE**: age at the time of the study.
 - **EDSS**: Expanded Disability Status Scale at the time of the study. 
 - **DATASET**: whether the subject was a part of the pilot or the consecutive project (is relevant because of the slight change in the fMRI acquisition parameters).
 - **DIAG_YEARS**: number of years since diagnosis.
 - **BMI**: BMI at the time of the study.
 - **THERAPY**: type of rehabilitation (see [Prochazkova et al 2020][2]).
 - **outliers_V1**: the absolute number of volumes flagged as outliers participant's first visit ([step 3][3] of the CONN pipeline).
 - **outliers_V2**: the absolute number of volumes flagged as outliers participant's second visit ([step 3][3] of the CONN pipeline).
----------
**nifti**

The directory contains [CONN][4] preprocessed fMRI time-series. Each subject was recorded twice - before and after neuroproprioceptive "facilitation and inhibition" treatment. 

----------
**quality measures**

Contains files with the appropriate displacement measures for each subject and visit.
 - **DVARS.csv** 
 - **FD.csv**

----------
**FC**

Contains functional connectivity matrices as **.csv* for each subject and visit.
Also contains file **AAL_labels.csv** with labels of AAL atlas regions.

----------
For more work of our **COBRA** group, please visit our [website][5]


  [1]: https://www.frontiersin.org/articles/10.3389/fnins.2021.662784/full
  [2]: https://journals.lww.com/intjrehabilres/Abstract/2015/03000/Motor_programme_activating_therapy_influences.6.aspx
  [3]: https://web.conn-toolbox.org/home
  [4]: https://web.conn-toolbox.org/fmri-methods/preprocessing-pipeline
  [5]: http://cobra.cs.cas.cz/