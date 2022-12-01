# Folder structure

This is a repo explaining how to make a standardized folder structure to organize your project and pipelines.

## In the future

... this repository will contain scripts that automate the folder_structure procedure once it has been agreed upon.

## Software for making ASCII tree folder structure.

To make a folder structure use the [link](https://codepen.io/weizhenye/details/eoYvye) and write your folder structure in hashtag-form. Alternatively copy the hashtag form below and modify it.

    Paste the input and output from the ASCII-tree generator and explain your structure!

Also, there is an vscode-plugin, that can do this directly in markdown in vscode: `ascii-tree-generator` from aprilandjan

### input

```
# project_name/
## README.md
## data/
### README.md
### metadata/
### raw_data/
### production_data/
## scripts/
## subprojects/
### awesome_project/
#### README.md
#### data/
##### production_data/
###### symlink
##### production_data_subset/
##### metadata/
#### results
#### scripts/

```

### output with

```
.
└── project_name/                # project name such as microflora_danica
    ├── README.md                # readme briefly explaining contents of main responsible
    ├── data/                    # main data folder
    │   ├── README.md            # explaination of data, dataprocessing, and guidelines for file naming and minimal metadata requirements
    │   ├── metadata/            # metadata
    │   ├── raw_data/            # raw data
    │   └── production_data/     # data ready for production
    ├── scripts/                 # scripts/pipelines used for making production_data
    └── subprojects/             # subproject folder
        └── awesome_project/     # Awesome subproject such as deep_metagenomes for soil
            ├── README.md        # Description of project and data analysis. Contains main responsible
            ├── data/            # data used in subproject
            │   ├── production_data/
            │   │   └── symlink  # symlink to production_data
            │   ├── production_data_subset/
            │   └── metadata/
            ├── results/         # results
            └── scripts/         # scripts for making results

```
