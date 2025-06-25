# List of Historic Microlensing events

The fields in Euclid Galactic Bulge Survey have been observed by historic surveys OGLE, MOA and KMTNet since the early 2000's. In this repository we include all the information we have collected on these historic events, providing predictions for the lens-source separation as it should be observed in EGBS images.

This work is being performed by V. Bozza, L. Salmeri and P. Rota (University of Salerno), in collaboration with the Euclid swg-exoplanets.

## Fieldcoords.txt

This file contains the list of the corners of each subquadrant in the images in the EGBS. The columns are:
- File name
- Subquadrant
- RA corner 1
- Dec corner 1
- RA corner 2
- Dec corner 2
- RA corner 3
- Dec corner 3
- RA corner 4
- Dec corner 4

## Whichfields.ipynb

A simple jupyter notebook to retrieve the fields in which we can find an object at given (ra,dec).
For a given (ra,dec) we obtain the list of image names and subquadrants in which we can find the object.

In the next cell, we can also obtain the pixel coodinates in each of the subquadrants.

Consider that the astrometry is only approximate because it only implements a linear transformation from the information found in the header. There might be discrepancies of the order of tens of pixel from the real position.

## HistoricList.txt

The list of all historic microlensing events in EGBS from OGLE, MOA and KMTNet with their information.
The total amounts to 8081 events. For each event we have the following columns:
- Event name
- Percentage_180: Percent probability that the lens is separated by more than 180 mas from the source
- Percentage_110: Percent probability that the lens is separated by more than 110 mas from the source
- Percentage_55: Percent probability that the lens is separated by more than 55 mas from the source
- Percentage_27_5: Percent probability that the lens is separated by more than 27.5 mas from the source
- Model: Best model category as found by RTModel
- tE: Einstein time
- err_tE: error on Einstein time
- I_baseline: I-band magnitude at the baseline (if available)
- t0: Time of closest approach between lens and source in HJD
- piEN: Microlensing parallax, North component
- err_piEN: Error on North component
- piEE: Microlensing parallax, East component
- err_piEE: Error on East component
- Extinction: Extinction in I-band
- RA: Right Ascension in degrees
- Dec: Declination in degrees
- chi2/dof: chi square over degrees of freedom as found by RTModel


## Real_fields_and_events.png

This image contains a plot of the EGBS fields with all historic microlensing events found in the fields.

# Current work

We are re-modeling all historic microlensing events in order to have a homogeneous set of parameters.

# Coming next

We will run [genulens](https://github.com/nkoshimoto/genulens) with constraints derived from our models to obtain predictions on the proper motions of all events
