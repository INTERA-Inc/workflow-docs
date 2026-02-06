title: 2. Python Environment

## Create Environment
- Create new python environment (using env.yml file)
- Create new plain text *.yml* file (example below) in root folder
- Note update `env_name`

``` { .yml }
    name: env_name
    channels:
      - conda-forge
    dependencies:
      - python=3.12
      - pip
      - numpy
      - pandas
      - matplotlib
      - plotly
      - geopandas
      - rasterio
      - shapely
      - pyproj
      - rtree
      - fiona
      - flopy
      - pyshp
      - pip:
          - mkdocs-material
          - mkdocs-awesome-pages-plugin
          - mkdocs-exclude
```

## Open VSCode and connect to project folder

-   File -> Open Folder
-   Open Terminal: CTRL+SHIFT+P -> Terminal: Create New Terminal
  
## Run below to create env (in anaconda prompt)

`mamba env create -f env.yml` or `conda env create -f env.yml

Suggest using 'mamba' as much faster solves and installs (parallel downloads)  

You may need to **deactivate ZScaler during the install**

Activate with `activate env_name` in CLI or select directly as interpreter in VSCode  

## Keep env updated after installing new packages

`mamba env export --from-history > env.yml`  
