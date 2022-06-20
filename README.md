# Spatial and Urban Data Science with PySAL @SciPy22

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sjsrey/pysal-scipy22/main)

### Instructors

-   [Sergio Rey](http://sergerey.org) - University of California, Riverside
-   [Elijah Knaap](https:/sjsrey.com) - University of California, Riverside

* * *

## Short Description

This repository contains the materials and instructions for the PySAL workshop at [SciPy 2022](https://www.scipy2222.scipy.org/).

Proposed Schedule:

-   Geographic Data Science with Python
    -   PySAL Overview
    -   Spatial data processing
    -   Choropleth mapping and geovisualization
        -   Break

-  Fundamentals of Spatial Analysis
    -   Spatial weights
    -   Global & Local spatial autocorrelation
        -   Break

-   Applied Spatial Analysis: Neighborhood Analytics
    -   Clustering/Geodemographic Analysis
    -   Segregation Analysis
        -   Break

-   Applied Spatial Analysis: Neighborhood Dynamics
    -   Modeling neighborhood change
    -   Measuring spatial and temporal segregation dynamics


## Long Description

### Fundamentals of Spatial Analysis

#### PySAL Overview

Brief introduction to the PySAL ecosystem of packages for spatial data science

#### Spatial data processing

Reading and writing GIS file formats, spatial data wrangling, changing coordinate transformation systems.

#### Choropleth mapping and geovisualization

Introduction to choropleth map classification using `mapclassify`. Basic visualization with GeoPandas, and matplotlib as well as interactive visualization via folium, leaflet and geoviews/hvplot,

_Hands-on 1 Exploratory Geovisualization_ 

#### Spatial weights

Introduction to the spatial weights matrix for formally encoding geographic relationships.

#### Global & Local spatial autocorrelation

Exploratory spatial data analysis and overview of measures of spatial autocorrelation statistics such as Moran's _I_ and the join-count statistic.

_Hands-on 2 Hot-spot detection_ 

### Applied Spatial Analysis: Neighborhood Analytics

Exploring socio-spatial differentiation

#### Clustering/Geodemographic Analysis

Introduction to classic and spatially-constrained geodemographics (regionalization). This module provides an overview of integrating `scikit-learn` and `pysal` to develop socio-demographic cluster models that optionally include a spatial constraint.

_Hands-on 3 Defining Neighborhoods_

#### Segregation Analysis

Applied segregation analysis including the calculation of classic, multigroup, and spatial indices. This module also includes analysis of spatial segregation dynamics, and comparative inference


### Applied Spatial Analysis: Neighborhood Dynamics

#### Neighborhood Change

Introduction to `geosnap` for creating geodemographic typologies over time and modeling neighborhood transitions

#### Segregation Dynamics

Examine changes in income segregation over space and time


_Hands-on 4 Comparative segregation_

## Obtaining Workshop Materials

If you are familiar with GitHub, you should clone or fork this GitHub repository to a specific directory. Cloning can be done by:

```bash
git clone https://github.com/sjsrey/pysal-scipy22.git
```

If you are not using git, you can grab the workshop materials as a [zip file](https://github.com/sjsrey/pysal-scipy22/archive/refs/heads/main.zip).
Extract the downloaded zip file to a working directory for the workshop.

## Installation

We will be using a number of Python packages for geospatial analysis.

An easy way to install all of these packages is to use a Python distribution such as [Anaconda](https://www.anaconda.com/download/#macos). In this workshop we will use anaconda to build an [environment](https://conda.io/docs/user-guide/tasks/manage-environments.html) for **Python 3.9**. It does not matter which version of anaconda is downloaded. We recommend installing Anaconda 3.9.

Once you have installed Anaconda, open a terminal and change into the directory where you downloaded the tutorial materials and create the workshop environment with:

```bash
conda env create -f environment.yml
```

This will build a conda python 3.9 environment that sandboxes the installation of the required packages for this workshop so we don't break anything in your computer's system Python (if it has one).

This may take 10-15 minutes to complete depending on the speed of your network connection.

Once this completes, you can activate the workshop environment with:

```bash
conda activate pysal-workshop
```

You are ready for the workshop at this point.
