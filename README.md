# Non-native freshwater fish fauna in Flanders, Belgium

## Rationale

This repository contains the necessary files and information required to map the _Checklist of the non-native freshwater fish species in Flanders, Belgium_ (Verreycken et al. 2018) to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org). It includes both the raw data file and the Darwin Core output, together with a human and machine-readable script to map the checklist data and the code for a [one-page website](http://trias-project.github.io/alien-fishes) to explore the data. It also contains the syntax to express the data specifications for the Darwin Core output files. This repository was developed for the [TrIAS project](http://trias-project.be).

The mapping script serves as the stepwise guide and description of the mapping process. It contains human-readable text combined with machine-readabe chuncks of code and is the core document to comprehend the transformation of the raw data to the Darwin Core Archive.

# Input

* [Raw data file](https://github.com/trias-project/alien-fishes/tree/master/data/raw)


## Code

* Description of the [Darwin Core mapping](https://github.com/trias-project/alien-fishes/tree/master/src/dwc_checklist.Rmd)
* [Data specifications](https://github.com/trias-project/alien-fishes-checklist/tree/master/specification) for the Darwin Core output files

## Results

* Generated [Darwin Core files](https://github.com/trias-project/alien-fishes/tree/master/data/processed)
* Published [dataset on the IPT](https://ipt.inbo.be/resource?r=alien-fishes-checklist)
* Published [dataset on GBIF](https://www.gbif.org/dataset/98940a79-2bf1-46e6-afd6-ba2e85a26f9f)


## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/). Files indicated with `GENERATED` should not be edited manually.

├── README.md         : Top-level description of the project and how to run it
├── LICENSE           : Project license
├── .gitignore        : Files and folders to be ignored by git
│
├── data
│   ├── raw           : Source data, input for mapping script
│   └── processed     : Darwin Core output of mapping script GENERATED
│
├── docs			  : Code for one-page website GENERATED
│
├── specifications    : Data specifications for Darwin Core output (YAML)
│
└── src
    ├── dwc_checklist.Rmd   : Darwin Core mapping script, core functionality of this repository
    └──  src.Rproj          : RStudio project file