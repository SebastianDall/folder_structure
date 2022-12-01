# Folder structure

This is a repo explaining how to make a standardized folder structure to organize your project and pipelines.

## In the future

... this repository will contain scripts that automate the folder_structure procedure once it has been agreed upon.

## Software for making ASCII tree folder structure.

To make a folder structure use the [link](https://codepen.io/weizhenye/details/eoYvye) and write your folder structure in hashtag-form.

paste the input and output from the ASCII-tree generator and explain your structure.

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
#### scripts/

```

### output

```
project_name/
├── README.md
├── data/
│   ├── README.md
│   ├── metadata/
│   ├── raw_data/
│   └── production_data/
├── scripts/
└── subprojects/
    └── awesome_project/
        ├── README.md
        ├── data/
        │   ├── production_data/
        │   │   └── symlink
        │   ├── production_data_subset/
        │   └── metadata/
        └── scripts/
```
