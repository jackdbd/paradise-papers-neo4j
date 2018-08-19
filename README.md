# Paradise Papers with Neo4j, Altair and Folium

Data exploration and visualization of the Paradise Papers dataset.

![A screenshot of the interactive map](https://github.com/jackdbd/paradise-papers-neo4j-folium/blob/master/screenshots/map-screenshot.png "Screenshot of the Folium map")

![A GIF that shows how to use the interactive map](https://github.com/jackdbd/paradise-papers-neo4j-folium/blob/master/screenshots/map-demo.gif "Demo of the Folium map")

![5 most popular offshore jurisdictions](./screenshots/popular-offshore-jurisdictions.svg, "popular-offshore-jurisdictions")


## Installation

If you want to run the notebook locally, you can create a conda environment.

Create and activate a new conda environment:

```
conda create --name paradise-papers python=3.6 --yes
source activate paradise-papers
```

Install all the dependencies (this might take a while, go grab a cup of coffee):

```sh
conda install -c conda-forge jupyter neo4j-python-driver pandas altair folium -y
```

*Note:* you don't need to install Neo4j. The notebook connects to a Neo4j sandbox that should be always available.


## Usage

When all dependencies have been installed, run the notebook:

```sh
jupyter notebook
```


## Misc
You can freeze your environment with:

```sh
conda env export > environment.yml
```

To remove this conda environment, run:

```sh
conda env remove -n paradise-papers -y
```


## Credits

This work was inspired by [William Lyon's tutorial](https://www.lyonwj.com/2017/11/28/geocoding-paradise-papers-neo4j-spatial-visualization/).

The [Paradise Papers dataset](https://offshoreleaks.icij.org/pages/database) is released by The International Consortium of Investigative Journalists. The dataset is licensed under the [Open Database License](https://opendatacommons.org/licenses/odbl/1.0/) and its contents under [Creative Commons Attribution-ShareAlike license](https://creativecommons.org/licenses/by-sa/3.0/).
