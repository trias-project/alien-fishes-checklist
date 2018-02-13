# Checklist of non-native freshwater fishes in Flanders, Belgium

## Rationale

This repository contains the functionality to standardize the _Checklist of non-native freshwater fishes in Flanders, Belgium_ (Verreycken et al. 2018) to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org). It was developed for the [TrIAS project](http://trias-project.be).

## Results

### Data

* Input: [source data](data/raw)
* Output: generated [Darwin Core files](data/processed)

### Mapping to Darwin Core

* Description of the [Darwin Core mapping](http://trias-project.github.io/alien-fishes) (= a rendition of the [mapping script](src/dwc_checklist.Rmd))
* [Data specifications](specification) for the Darwin Core files

### Published dataset

* [Dataset on the IPT](https://ipt.inbo.be/resource?r=alien-fishes-checklist)
* [Dataset on GBIF](https://doi.org/10.15468/xvuzfh)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/). Files indicated with `GENERATED` should not be edited manually.

```
├── README.md         : Top-level description of the project and how to run it
├── LICENSE           : Project license
├── .gitignore        : Files and folders to be ignored by git
│
├── data
│   ├── raw           : Source data, input for mapping script
│   └── processed     : Darwin Core output of mapping script GENERATED
│
├── docs              : Code for one-page website GENERATED
│
├── specifications    : Data specifications for the Darwin Core files
│
└── src
    ├── dwc_checklist.Rmd   : Darwin Core mapping script, core functionality of this repository
    └── src.Rproj          : RStudio project file
```
