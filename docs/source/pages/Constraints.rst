###########
Constraints
###########

Product quality
***************
The quality of the Sentinel-2 Global Mosaic data is depending on the quality of the official Sentinel-2 L2A products used as inputs.
The S2GM Mosaic Hub utilizes the products as they are provided by the Copernicus service, including the contained scene
classification. Deficits (commission and omission errors) in the quality of the scene classification affect the outputs
of the Mosaic Hub.

**Known Issues**

* Cloud border often visible (especially short periods)
* Swath boarder artefacts
* Replaced clouds are visible caused by exchanged surface reflectance values
* Selection of undetected  or clouds classified as snow

1 Mio square km direct order limit
**********************************
In case the bounding box of the order area includes more than 1 million km², product size will be very large and processing time may
be considerable. In this case, we will get in touch with you in order identify the best way of production scheduling and
product distribution.

Minimum bandwidth of 200 Mbit/s
*******************************
The S2GM Mosaic Hub provides a minimum bandwidth of 200 Mbit/s for the data download.
The bandwidth is shared by all simultaneous downloads.