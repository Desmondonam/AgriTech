"# AgriTech" 
This Python package allows us to retrieve, manipulate, and visualize point data. The main features of the package are the following.

The ability to accept a field boundary polygon in a geopandas dataframe in any coordinate reference system (CRS) and a desired output CRS and return a python dictionary with all available years of data and a geopandas grid point file with elevations encoded in the requested coordinate reference system (CRS).
The ability to provide an option to graphically display the returned elevation files as either a 3D render plot or a heatmap.
The ability to apply data transformation and return additional data such as Topographic wetness index (TWI) and Standardized grid.
# Dependancies
This package is dependent on the following python packages.

1. PDAL
2. Laspy
3. Geopandas


# Business Need
At AgriTech, we are very interested in how water flows through a maize farm field. This
knowledge will help us improve our research on new agricultural products being tested on
farms.
How much maize a field produces is very spatially variable. Even if the same farming
practices, seeds and fertilizer are applied exactly the same by machinery over a field, there
can be a very large harvest at one corner and a low harvest at another corner. We would
like to be able to better understand which parts of the farm are likely to produce more or
less maize, so that if we try a new fertilizer on part of this farm, we have more confidence
that any differences in the maize harvest 9are due mostly to the new fertilizer changes, and
not just random effects due to other environmental factors.
Water is very important for crop growth and health. We can better predict maize harvest if
we better understand how water flows through a field, and which parts are likely to be
flooded or too dry. One important ingredient to understanding water flow in a field is by
measuring the elevation of the field at many points. The USGS recently released high
resolution elevation data as a lidar point cloud called USGS 3DEP in a public dataset on
Amazon. This dataset is essential to build models of water flow and predict plant health and
maize harvest.
You work at an AgriTech, which has a mix of domain experts, data scientists, data engineers.
As part of the data engineering team, you are tasked to produce an easy to use, reliable and
well designed python module that domain experts and data scientists can use to fetch,
visualise, and transform publicly available satellite and LIDAR data. In particular, your code
should interface with USGS 3DEP and fetch data using their API.
You may search for open source python packages and adapt them to your needs, or you
may choose to write everything from scratch. In the former case, please be clear about
attributing where the work and code came from - this is essential.
The quality of your python package is judged by
● How easy it is to install and use
● How much abstraction it exposes - from high level - a few function calls to do all
routine work, to low level - gives a high degree of control to users.
● CPU and RAM usage
● Implementation of parallelisation to speed up fetching, loading, transforming, and
visualization.
You may not have time to implement all these elements this week, but you may write your
code thinking about future implementation of these and other useful features.