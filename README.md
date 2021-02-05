# leiden
_cluster graph(s) with the leiden algorithm_

## Usage

This is a wrapper script around `vtraag's` [Leiden Algorithm](https://github.com/vtraag/leidenalg). Put this script in your path, and then you can call from anywhere!

```bash

# cluster a graph with the surprise algorithm
leiden adjm.csv -q Surprise 

# NOTE: currently only supports a single resolution!

leiden adjm.csv -q CPM -g 1
```

## Dependencies
I recommend using a virtual environment such as conda:
* leidenalg -- `conda install -c conda-forge leidenalg`
* igraph -- `conda install -c conda-forge leidenalg`
