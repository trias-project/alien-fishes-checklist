# Checklist of non-native freshwater fishes in Flanders, Belgium

## Rationale

This repository contains the functionality to standardize the _Checklist of non-native freshwater fishes in Flanders, Belgium_ (Verreycken et al. 2018) to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org). It was developed for the [TrIAS project](http://trias-project.be).

## Workflow

[source data](https://github.com/trias-project/alien-fishes-checklist/blob/master/data/raw) → Darwin Core [mapping script](http://trias-project.github.io/alien-fishes-checklist/dwc_mapping.html) → generated [Darwin Core files](https://github.com/trias-project/alien-fishes-checklist/blob/master/data/processed)

## Published dataset

* [Dataset on the IPT](https://ipt.inbo.be/resource?r=alien-fishes-checklist)
* [Dataset on GBIF](https://doi.org/10.15468/xvuzfh)

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md         : Description of this repository
├── LICENSE           : Repository license
├── .gitignore        : Files and directories to be ignored by git
│
├── data
│   ├── raw           : Source data, input for mapping script
│   └── processed     : Darwin Core output of mapping script GENERATED
│
├── docs              : Repository website GENERATED
│
├── specifications    : Data specifications for the Darwin Core files
│
└── src
    ├── dwc_mapping.Rmd : Darwin Core mapping script, core functionality of this repository
    └── src.Rproj       : RStudio project file
```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generated the processed data and build the website in `/docs`

## Contributors

[List of contributors](https://github.com/trias-project/alien-fishes-checklist/contributors)

## License

[MIT License](https://github.com/trias-project/alien-fishes-checklist/blob/master/LICENSE)
