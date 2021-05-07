# ARIWS-Cookbook
Beginners guide for introducing and training using MeerKAT data    
The cookbook forms part of the SARAO African Radio Interferometry Winter School (ARIWS)    
The winter school can be found online via [SARAO E-learning](https://www.sarao.ac.za/e-learning-portal/)

Practical examples and tutorials uses Google COLAB and can be executed online.    
Note: Data used in the tutorials must be uploaded to the notebooks during the processing runs

This notebook is for introduction purposes only, for more information please refer to the
[MeerKAT-Cookbook](https://github.com/ska-sa/MeerKAT-Cookbook), available through the SARAO
operational interface.
The MeerKAT cookbook contains notebooks with detailed examples specifically focused to MeerKAT user
interfacing, such as:
* How to interact with the SARAO archive
[MeerKAT-Cookbook/archive](https://github.com/ska-sa/MeerKAT-Cookbook/blob/master/archive)
* Using the MeerKAT `katdal` software to inspect, obtain and process MeerKAT data
[MeerKAT-Cookbook/katdal](https://github.com/ska-sa/MeerKAT-Cookbook/tree/master/katdal)
* As well as some MeerKAT specific notebooks for observation planning
[MeerKAT-Cookbook/utility](https://github.com/ska-sa/MeerKAT-Cookbook/tree/master/utility)

## CASA
Standard recipes for flagging and calibration    
CASA MeasurementSet data tables can be created using a convenient helper script `mvftoms.py` available
from `katdal` installation.     
Measurement sets can be downloaded directly from the MeerKAT archive using some sensible defaults when
created.
MeerKAT operational
Examples on how to create measurement sets from a user control environment using tokens from the
archive are given in example notebooks in the archive folder of the
[MeerKAT-Cookbook](https://github.com/ska-sa/MeerKAT-Cookbook).

## TUTORIALS
Introductory notebooks to familiarise the user with radio astronomy concepts and methods.    
All tutorials make extensive use of the `matplotlib` and `astropy` python libraries
```
pip install matplotlib
pip install astropy
```

Plotting the antenna location makes use of the `mpl_toolkits.basemap` functionality, which may be a little tricky to install.    
`Basemap` installation requires `libgeos`. The following worked for the author
```
sudo apt-get install libgeos-3.6.2 libgeos-c1v5 libgeos-dev
git clone https://github.com/matplotlib/basemap.git
cd basemap/
pip install .
```

 -fin-
