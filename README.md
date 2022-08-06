# mCIRCrna
The goal is to integrate circadian transcriptomes with muscle snRNA-seq data to identify age and cell type dependent circadian gene signatures that demonstrate tissue chronicity in muscle.


## Table of Contents

- [mCIRCrna](#team-repo-template)
    - [Background](#Background)
    - [Data](#data)
    - [Usage](#usage)
        - [Installation](#installation)
        - [Requirements](#requirements) _Can be named Dependencies as well_
        - [Activate conda environment](#activate-conda-environment) _Optional_
        - [Steps to run ](#steps-to-run) _Optional depending on project_
            - [Step-1](#step-1)
            - [Step-2](#step-2)
    - [Results](#results) _Optional depending on project_
    - [Team Members](#team-members)
## Purpose
To identify circadian gene signatures that demonstrate tissue chronicity (2 fold expression changes over time) compared to age and cell type in muscle.

## Aims
-Identify skeletal muscle circadian gene signatures that demonstrate tissue chronicity  (2 fold expression changes over time)
-Identify skeletal muscle cell types with differential circadian gene expression during aging  

## Abstract

Skeletal muscle is an endocrine organ that composes 40-60% of the adult body mass with overall health span implications for the entire body. Significant declines in circadian physiology and behavior is widely accepted as an aging-associated phenotype. In fact, age-dependent circadian transcriptomic reprogramming has recently been observed in the skeletal muscle.The cell-type specific expression of these genes however has not yet been characterized in the skeletal muscle. We hypothesize that in aging these genes that are expressed in a circadian manner could become dysregulated in a cell specific manner. 

In this project, we first acquired published circadian gene expression data (McCarthy et.al. 2007) from  mouse C57B6/J gastrocnemius muscle 7-10 weeks of age. We compared it to CircAge bulk transcriptomics of C57B6/J-NIA mice skeletal muscle which measured gene expression from tissue collected every 4 hours for 48 hours in total darkness (DD), with the first time point being circadian time (CT) 18. We used the 6 month (young adult) and 27 month (old-adult) data.

Next, we utilized snRNA-seq data that is represented in the graphical tool, myoatlas, from 5 month (young adult) and 24 month (old adult) tibia anterior (TA) data. We integrated the data across age for differential expression singularly and also inputted our significantly changing circadian rhythm to understand the potential for cell specific expression. 

Here we show that (main result goes here).

This suggests that (meaning of results)

This work can be cross referenced to disease datasets to better understand skeletal muscle cell localization of circadian rhythm gene expression in the context of aging. Understanding the circadian gene expressions in skeletal muscle cell types during aging could lead to precise drug targeting therapeutics that supports entire body health. 

## Data

-McCarthy JJ, Andrews JL, McDearmon EL, Campbell KS, Barber BK, Miller BH, Walker JR, Hogenesch JB, Takahashi JS, Esser KA. Identification of the circadian transcriptome in adult mouse skeletal muscle. Physiol Genomics. 2007 Sep 19;31(1):86-95. doi: 10.1152/physiolgenomics.00066.2007. Epub 2007 Jun 5. PMID: 17550994; PMCID: PMC6080860.

- CircAge: https://circaage.shinyapps.io/circaage/
- MyoAtlas: https://research.cchmc.org/myoatlas/

## Usage

To 

:exclamation: _How will someone not involved in your project be able to run the code or use it._ :exclamation:

### Installation

:exclamation: _If installation is required, please mention how to do so here._ :exclamation:

Installation simply requires fetching the source code. Following are required:

- Git

To fetch source code, change in to directory of your choice and run:

```sh
git clone -b main \
    git@github.com:u-brite/team-repo-template.git
```

### Requirements
:exclamation: _Note any software used (including Python or R packages), operating system requirements, etc. and its version so that your project is reproducible. It does not have to be in the below format_ :exclamation:

*OS:*

Currently works only in Linux OS. Docker versions may need to be explored later to make it useable in Mac (and
potentially Windows).

*Tools:*

- Anaconda3
    - Tested with version: 2020.02

### Activate conda environment
:exclamation: _Optional: Depends on project._ :exclamation:

Change in to root directory and run the commands below:

```sh
# create conda environment. Needed only the first time.
conda env create --file configs/environment.yaml

# if you need to update existing environment
conda env update --file configs/environment.yaml

# activate conda environment
conda activate testing
```

### Steps to run
:exclamation: _Optional: Depends on project._ :exclamation:

#### Step 1

```sh
python src/data_prep.py -i path/to/file.tsv -O path/to/output_directory
```

#### Step 2

```sh
python src/model.py -i path/to/parsed_file.tsv -O path/to/output_directory
```

Output from this step includes -

```directory
output_directory/
├── parsed_file.tsv               <--- used for model
├── plot.pdf- Plot to visualize data
└── columns.csv - columns before and after filtering step

```

**Note**: The is an example note with a [link](https://github.com/u-brite/team-repo-template).


## Results
:exclamation: _If your project yielded or intends to yield some novel analysis, please include them in your readme. It can be named something other than results as well._ :exclamation:

## Team Members

Shufan Zhang | shufan0519@gmail.com | Team Leader  

