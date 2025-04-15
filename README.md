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

A simple jupyter notebook to find the fields in which we can find an object at given (ra,dec).
For a given (ra,dec) we obtain the list of images and subquadrants in which we can find the object.
In the nxt cell, we can also obtain the pixel coodinates in each of the subquadrants.

Consider that the astrometry is only approximate with a linear transformation. There might be a discrepancy of tens of pixel with the correct position.

## Real_fields_and_events.png

This image contains a plot of the EGBS fields with all historic microlensing events found in the fields.

## HistoricList.txt

The list of all historic microlensing events found in EGBS with their parameters extracted from OGLE, MOA or KMTNet web pages.

# Current work

We are re-modeling all historic microlensing events in order to have a homogeneous set of parameters.

# Coming next

We will run [genulens](https://github.com/nkoshimoto/genulens) with constraints derived from our models to obtain predictions on the proper motions of all events
