# Paradise Papers with Neo4j and Python Folium

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/jackdbd/paradise-papers-neo4j-folium/master)

TODO: description

TODO: screenshot/GIF


## Run the notebook with Binder

[Binder](https://github.com/jupyterhub/binderhub) builds a docker image from a git repository + commit, so you can run the notebook beni-confiscati.ipynb in the cloud, without installing anything on your machine.


## Installation

If you want to run the notebook locally, you need to create a conda environment. You can use either Miniconda or Anaconda.

Create and activate a new conda environment:

conda create --name paradise-papers python=3.6 --yes
source activate paradise-papers
Install all the dependencies (this might take a while, go grab a cup of coffee):

```sh
conda install -c conda-forge jupyter python-dotenv pandas matplotlib neo4j-python-driver folium -y
```

## Usage

When all dependencies have been installed, run the notebook:

```sh
jupyter notebook
```

Start the Neo4j daemon with:

```sh
sudo service neo4j start
```

Check that Neo4j is up and running by visiting:

```
http://localhost:7474/browser/
```


## Misc
You can freeze your environment with:

```sh
conda env export > environment.yml
```

To remove this conda environment, run:

```sh
conda env remove -n paradise-papers
```


## Credits

Inspired by [William Lyon's article](https://www.lyonwj.com/2017/11/28/geocoding-paradise-papers-neo4j-spatial-visualization/).
