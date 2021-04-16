# leiden
_cluster graph(s) with the leiden algorithm_

## Usage

This is a wrapper script around `vtraag's` [Leiden
Algorithm](https://github.com/vtraag/leidenalg). Put this script in your path,
and then you can call it from anywhere!

```bash

# get a graph
wget https://github.com/twesleyb/leiden/raw/master/data/adjm.zip

unzip adjm.zip && cd adjm/

# cluster the graph with the leiden algorithm and surprise
leiden adjm.csv -q Surprise 

# or try the CPM algorithm
leiden adjm.csv -q CPM -g 1

# NOTE: currently only supports a single resolution!
```

## Dependencies
I recommend using a virtual environment such as `conda`. Then insure you have
installed the following python dependencies:
* _leidenalg_ 
* _igraph_
```
conda install -c conda-forge igraph leidenalg
```
