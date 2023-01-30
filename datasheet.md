# Datasheet

The dataset used in this repository is the one referenced in Rieth et al. (2017), Issues and Advances in Anomaly Detection Evaluation for Joint Human-Automated Systems. 

## Motivation

- This datasource contains the data referenced in [Rieth et al. (2017)](https://doi.org/10.7910/DVN/6C3JR1), Issues and Advances in Anomaly Detection Evaluation for Joint Human-Automated Systems. To be presented at Applied Human Factors and Ergonomics 2017.
- The work in [Rieth et al. (2017)](https://doi.org/10.7910/DVN/6C3JR1) was sponsored by the Office of Naval Research, Human & Bioengineered Systems (ONR 341), program officer Dr. Jeffrey G. Morrison under contract N00014-15-C-5003. 

 
## Composition

The original datasource is represented in .RData format. Each datafile is an external representation of an R dataframe that can be read into an R environment with the ‘load’ function. Here, for simplicity, we use a sample of this source converted in csv format.

Each dataframe contains 55 columns:

Column 1 (‘faultNumber’) ranges from 1 to 20 in the “Faulty” datasets and represents the fault type in the TEP. The “FaultFree” datasets only contain fault 0 (i.e. normal operating conditions).

Column 2 (‘simulationRun’) ranges from 1 to 500 and represents a different random number generator state from which a full TEP dataset was generated (Note: the actual seeds used to generate training and testing datasets were non-overlapping).

Column 3 (‘sample’) ranges either from 1 to 500 (“Training” datasets) or 1 to 960 (“Testing” datasets). The TEP variables (columns 4 to 55) were sampled every 3 minutes for a total duration of 25 hours and 48 hours respectively. Note that the faults were introduced 1 and 8 hours into the Faulty Training and Faulty Testing datasets, respectively.

Columns 4 to 55 contain the process variables; the column names retain the original variable names.

We use a random sample (30%) of the original datasource. There is no missing data values. The dataset does not contain confiential information.

## Collection process

The generation of the original dataset is described in [Rieth et al. (2017)](https://doi.org/10.7910/DVN/6C3JR1). The dataset used here was randomly sampled from the original dataset.
The original dataset was published in July 6, 2017.

## Preprocessing/cleaning/labelling

To the best of our knowledge no preprocessing has been carried out.
 
## Uses

The dataset was created for benchmarking anomaly detection algorithms of industrial process control systems.


## Distribution

The original dataset is distributed under Custome Dataset Terms. The terms of use can be found [here](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/6C3JR1&version=1.0&selectTab=termsTab).


## Maintenance

The dataset is maintained by [Harvard Dataverse](https://dataverse.harvard.edu/).

