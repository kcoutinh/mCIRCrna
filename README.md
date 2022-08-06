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
    - [Team Members] Lisa Shresta, Van Nha Huynh, Kristen Coutinho, Russel Santos, Herminio Vazquez, Shufan Zhang
## Purpose
To identify circadian gene signatures that demonstrate tissue chronicity (2 fold expression changes over time) compared to age and cell type in muscle.

## Aims
- Identify skeletal muscle circadian gene signatures that demonstrate tissue chronicity  (2 fold expression changes over time)
- Identify skeletal muscle cell types with differential circadian gene expression during aging  

## Abstract

Skeletal muscle is an endocrine organ that composes 40-60% of the adult body mass with overall health span implications for the entire body. Significant declines in circadian physiology and behavior is widely accepted as an aging-associated phenotype. In fact, age-dependent circadian transcriptomic reprogramming has recently been observed in the skeletal muscle.The cell-type specific expression of these genes however has not yet been characterized in the skeletal muscle. We hypothesize that in aging these genes that are expressed in a circadian manner could be expressed in a cell specific manner. 

In this project, we first acquired published circadian gene expression data (McCarthy et.al. 2007) from  mouse C57B6/J gastrocnemius muscle 7-10 weeks of age (young). We compared it to CircAge bulk transcriptomics of C57B6/J-NIA mice skeletal muscle which measured gene expression from tissue collected every 4 hours for 48 hours in total darkness (DD), with the first time point being circadian time (CT) 18. We used the 6 month (young adult) and 27 month (old-adult) data.

Next, we utilized snRNA-seq data from tibia anterior (TA) that is represented in the graphical tool, Myoatlas, from 5 month (young adult) and 24 month (old adult) data. With Seurat version 4.1.1 and the preprocessed count data from Synapse, we integrated the data across age for differential expression singularly.

To understand the potential for circadian related cell specific expression, we compared our significantly changing circadian rhythm genes aqcuired from CircAge (6 and 27 months) to our significantly changing cell-specific genes from Synapse (5 and 24 months). 

Here we show that (main result goes here).

This suggests that (meaning of results)

This work can be cross referenced to disease datasets to better understand skeletal muscle cell localization of circadian rhythm gene expression in the context of aging. Understanding the circadian gene expressions in skeletal muscle cell types during aging could lead to precise drug targeting therapeutics that supports entire body health. 

## Data

- McCarthy JJ, Andrews JL, McDearmon EL, Campbell KS, Barber BK, Miller BH, Walker JR, Hogenesch JB, Takahashi JS, Esser KA. Identification of the circadian transcriptome in adult mouse skeletal muscle. Physiol Genomics. 2007 Sep 19;31(1):86-95. doi: 10.1152/physiolgenomics.00066.2007. Epub 2007 Jun 5. PMID: 17550994; PMCID: PMC6080860.
- CircAge: https://circaage.shinyapps.io/circaage/
- MyoAtlas: https://research.cchmc.org/myoatlas/
- 5 month MyoAtlas prepocessed data: https://www.synapse.org/#!Synapse:syn21694348
- 24 month MyoAtlas preprocessed data: https://www.synapse.org/#!Synapse:syn21694476

## Usage

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

Useable in Mac and Windows.
 
*Tools:*

- R
    - Tested with version: 4.1.1
-R studio
    - Tested with version: 

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

