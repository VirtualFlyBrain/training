# Tools landscape
There are multiple tools to query the various data sources. Fortunately
they play together nicely. Here is a quick overview:

<p align="center">
<img src="https://github.com/VirtualFlyBrain/training/raw/main/presentations/_static/vfb_workshop.png" width="600">
</p>

Below are brief descriptions of the libraries/packages. For details, I defer
to their respective (excellent) documentations.

## Querying VFB
Queries against VFB's REST API are easiest with
[`vfb_connect`](https://github.com/VirtualFlyBrain/VFB_connect) for Python.
For R there is a `vfb_connect` wrapper ,
[`vfbconnectr`](https://github.com/jefferis/vfbconnectr) using reticulate.
See also David's presentation for details.

## R
In R the [natverse](http://natverse.org) is your one-stop-shop for all things
neuron: it's a collection of various R packages that are built on top of
the **n**euro**a**natomy **t**oolbox, `nat`. Of particular relevance for
this workshop:

1. [`nat`](http://natverse.org/nat/) is a general purpose library for working
   with morphological neuron data. In this workshop, we make heavy use of
   `nat`'s plotting capabilities but its capabilities extend far beyond that.
    If you want to run any morphological analysis, I highly recommend
   you have a look at the "Articles" in nat's [doc](http://natverse.org/nat/).
2. [`neuprintr`](http://natverse.org/neuprintr/reference/) and
   [`hemibrainr`](http://natverse.org/hemibrainr/) provide an interface with
   neuprint and the Janelia hemibrain dataset
   ([link](https://neuprint.janelia.org)). The former lets you run queries
   against neuprint's neo4j database while the latter contains meta data
   and various convenience functions to work with the hemibrain dataset.
3. [`rcatmaid`](http://natverse.org/rcatmaid/) provides an interface with
   CATMAID servers such as those the VFB uses to host published from the
   FAFB or larval fruit fly dataset.    

## Python
In Python we packages analogous to those in R:

1. [`navis`](https://navis.readthedocs.io/en/latest/) is `nat`'s serpentine
   sibling: a general purpose neuron library for visualization and analysis
   of neuronal morphologies. It also features interfaces with


## Other noteworthy mentions
There are a few more packages that you might hear of

<p align="center">
<img src="https://github.com/VirtualFlyBrain/training/raw/main/presentations/_static/vfb_workshop2.png" width="600">
</p>
