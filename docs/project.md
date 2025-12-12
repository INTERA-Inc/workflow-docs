## General folder structure suggestion

    root (e.g. project-name)
    │
    ├── data               -model data
    │   ├── raw            -original/unedited data
    │   └── processed      -processed/model ready data
    ├── docs               -model documentation (md files)
    │   ├── decisions      -decision log
    │   ├── report         -report (exported using template format)
    │   └── runs           -run log
    ├── modl               -main model folder
    │   ├── ss             -steady state model, input/output
    │   │   ├── XXX_1.0    -steady model files, versioned
    │   │   └── XXX_2.0
    │   │       ...
    │   └── trans          -transient model, input/output
    │       └── XXX_1.0    -transient model files, versioned
    │           ...
    ├── model_input        -model inputs read by workflow (e.g. obs data, CSVs)
    ├── nb_helpers         -support notebooks (e.g. pre-processing)
    ├── util               -utilities and manual
    ├── ss                 -superseded
    │
    ├── wb01_xxx.ipy       -model build, run and pest notebooks (main nbs)
    └── wb02_xxx.ipynb
        ...

Use the following command in a CLI to create the folder structure  

    mkdir data\raw data\processed docs\decisions docs\report docs\runs modl\ss modl\transient model_input nb_helpers util ss