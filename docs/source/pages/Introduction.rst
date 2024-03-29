.. _intro:

############
Introduction
############


.. image:: images/SouthernFranceY2017_60m.png
   :width: 75%
   :align: right

The Sentinel-2 Global Mosaic service offers mosaic surface reflectance products derived from the Sentinel-2 A and B platforms.
Input to the processing is the Level 2A (L2A) products provided by the Copernicus Ground Segment, i.e. ESA Sentinel-2 core products.
The S2GM service generates regional and temporal composites at global scale and produced on-demand over specific areas of interest.
Mosaics consist of best representative spectra for a given pixel location and compositing period, ensuring the consistency of spectra and thus the radiometric quality of the products.

The mosaics can be configured with the following options:

* Compositing Period: Year, Quarter, Month, Ten Days, Day
* Image Format: Geo Tiff, JPEG 2000, NetCDF
* Resolution: 10m, 20m, 60m
* Coordinate System: WGS 84, UTM

Users of the Sentinel-2 Global Mosaic (S2GM) service benefit from a convenient configuration and request process in the Mosaic Hub,
the powerful user interface to the service, and the analysis-ready products, which allow for instant further thematic processing.

This manual enables new users of the Sentinel-2 Global Mosaic to fully exploit the capabilities of the service.
It contains a guide on the usage of :ref:`mosaic_hub`, an overview of the :ref:`mosaic_algos` used to generate mosaics, and a :ref:`prod_guide`,
which elaborates on content, format, and usage of the mosaics. In addition to this user manual, expert users are referred to the [S2GMATBD]_.

For any questions that remain unanswered by this document or any other issues S2GM users are kindly
referred to the `User Support <https://s2gm.sentinel-hub.com/node/6>`_. We are keen to learn more about your experiences to
further improve the Sentinel-2 Global Mosaic service!
