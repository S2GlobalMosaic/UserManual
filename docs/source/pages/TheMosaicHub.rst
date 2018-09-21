.. _mosaic_hub:

##############
The Mosaic Hub
##############

The Mosaic Hub front-end is the main tool for S2GM users.
It allows to specify S2GM products in terms of the spatial extent as well as the compositing period
and the format of the output products. The front-end guides the user through the process of this product specification.
A registration is required before requesting and downloading mosaics.


Registration
************
For the registration process, guide your browser to the `Subscription Page <https://services.sentinel-hub.com/oauth/subscription>`_.
After you have filled out the form (see :numref:`mosaicHubRegistration`), you will receive an e-mail to confirm your
mail address. Click on the verification button and you will receive the confirmation that your account has been created.

.. _mosaicHubRegistration:
.. figure:: images/MosaicHubRegistration.png
   :name: mosaicHubRegistrationName
   :scale: 50%
   :alt: Mosaic Hub Registration
   :align: center

   Mosaic Hub Registration


.. _order:

Mosaic Ordering
***************
This page describes the process of ordering  mosaics, from defining the conditions to the download of the processed product.
The ordering of :ref:`time_series` is described below.

Mosaic Hub
==========

The Mosaic Hub is located `here <https://webdev.sentinel-hub.com/mosaic-hub/#/>`_.

However, in order to download the processed products, you will have to install the "Mosaic Downloader" App.
In fact, this App has the same functionality like the browser instance. In order to avoid switching between browser and
Mosaic Downloader, it might be more convenient to work with the App from the beginning.


Mosaic Downloader
=================
In the Mosaic Hub, click on the drop-down menu item "Mosaic Downloader" like in :numref:`mosaicDownloaderMenu`.

.. _mosaicDownloaderMenu:
.. figure:: images/MosaicDownloaderMenu.png
   :name: mosaicDownloaderMenuName
   :scale: 50%
   :alt: Mosaic Downloader Menu Item
   :align: center

   Mosaic Downloader Menu Item

From there, you are able to download the App for your specific OS, or even launch the App from the browser menu.
When you launch the App, you will see a window like in :numref:`mosaicDownloaderAppBase`.

.. _mosaicDownloaderAppBase:
.. figure:: images/MosaicDownloaderAppBase.png
   :name: mosaicDownloaderAppBaseName
   :scale: 50%
   :alt: Mosaic Downloader App Window (Base view)
   :align: center

   Mosaic Downloader App Window (Base view)

.. _mosaicDownloaderAppS2:
.. figure:: images/MosaicDownloaderAppS2.png
   :name: mosaicDownloaderAppS2Name
   :scale: 50%
   :alt: Mosaic Downloader App Window (Sentinel view)
   :align: center

   Mosaic Downloader App Window (Sentinel view)

The menu of the App on the top will bring up the following functionality after clicking:

.. .. todo::
   Replace TBD with content. Discuss with Sinergise what shall be behind the links.

+------------------------+------------------+
| Menu Button            |  Functionality   |
+========================+==================+
| Home                   | TBD              |
+------------------------+------------------+
| User Manual            | This document    |
+------------------------+------------------+
| User Area              | Status of Orders |
+------------------------+------------------+
| Mosaic Hub             | Configuration    |
|                        | of Mosaics       |
+------------------------+------------------+
| Time Series            | Configuration    |
|                        | of Time Series   |
+------------------------+------------------+
| Mosaic Downloader      | Configuration    |
|                        | and Execution    |
|                        | of Downloads     |
+------------------------+------------------+
| Resources              | TBD              |
+------------------------+------------------+
| About S2GM             | TBD              |
+------------------------+------------------+


The App Window is split with the dynamic map on the right and the temporal and spatial
configuration options on the left. Users can scroll and zoom into the map to focus on an area of interest.


Area Selection
--------------

.. _areaSelection:
.. figure:: images/AreaSelection.png
   :name: areaSelectionName
   :scale: 100%
   :alt: Area Selection
   :align: center

   Area Selection

As depicted in :numref:`Fig. {number}: {name} <areaSelection>`, several options exist to define the area for which the mosaic product will be generated (Note: Your product might be split into several tiles if it spans a large area - see also the warning displayed on :numref:`orderPanelOrder`):

* Drawing a rectangular or a polygon of arbitrary geometry on the map after selecting the corresponding icon in the menu on the upper right of the map (see :numref:`drawingTools`)
* Uploading a kml or kmz shape file; the upload button is located on the second tab in the area selection menu of the configuration menu
* Selection of a pre-defined area, i.e. a country or a continent, in the dropdown menus of the configuration menu
* Entering the area boundaries in WKT format (see :numref:`Fig. {number}: {name} <WKT>`; note that in WKT the first and last co-ordinates must be identical to close the polygon


.. _drawingTools:
.. figure:: images/DrawingTools.png
   :name: drawingToolsName
   :scale: 100%
   :alt: Drawing Tools
   :align: center

   Drawing Tools

.. _WKT:
.. figure:: images/WKT.png
   :name: wktName
   :scale: 75%
   :alt: WKT Example
   :align: center

   WKT Example


Compositing Periods
-------------------
The definition of the compositing period is done in the temporal period section of the configuration menu.
Five different compositing periods can be selected: year, season, month, 10-day, day.
For each of these compositing periods, pre-defined periods can be selected by choosing the desired option in the corresponding tabs.
Unavailable periods are disabled and marked in grey colour. In the 10-day and the day tabs, one can select months and years
from drop-down lists. The forward and backward scrolling can be done by clicking on the arrow symbol.

.. _compositingYear:
.. figure:: images/CompositingPeriodYear.png
   :name: compositingYearName
   :scale: 50%
   :alt: Compositing Dialog (Year)
   :align: center

   Compositing Dialog (Year)

As it can be seen in :numref:`compositingYear`, one can select a complete year as compositing period by clicking on it.

.. _compositingQuarter:
.. figure:: images/CompositingPeriodQuarter.png
   :name: compositingQuarterName
   :scale: 50%
   :alt: Compositing Dialog (Quarter)
   :align: center

   Compositing Dialog (Quarter)

Select a three-month period by clicking on the buttons Q1-Q4 (:numref:`compositingQuarter`).


.. _compositingMonth:
.. figure:: images/CompositingPeriodMonth.png
   :name: compositingMonthName
   :scale: 50%
   :alt: Compositing Dialog (Month)
   :align: center

   Compositing Dialog (Month)

The selection of the desired month as compositing period is straightforward (:numref:`compositingMonth`).

.. _compositing10Days:
.. figure:: images/Compositing10Days.png
   :name: compositing10DaysName
   :scale: 50%
   :alt: Compositing Dialog (10 days)
   :align: center

   Compositing Dialog (10 days)

The definition of a ten-day-period is bound to pre-defined, fixed intervals.
The latter are displayed on the specific tab. Start and end days are marked in dark green,
the intermediate values in light green (see :numref:`compositing10Days`). Clicking on either day in the interval yields the same result.

.. _compositingDay:
.. figure:: images/CompositingPeriodDay.png
   :name: compositingDayName
   :scale: 50%
   :alt: Compositing Dialog (Day)
   :align: center

   Compositing Dialog (Day)

The selection of the desired day as compositing period is straightforward (:numref:`compositingDay`).


Once the area of interest and compositing period have been selected, users must define further properties in the Order Panel dialogue.
Click on "**PREPARE DOWNLOAD**" to enter the Order Panel.


Order Panel
-----------
.. _orderPanel:

You will have to walk through four tabs and make your choices.
On the last tab, you will be able to resume your selections. In the first tab the data format has to be defined (see :numref:`orderPanelData`).

.. _orderPanelData:
.. figure:: images/OrderPanelData.png
   :name: orderPanelDataName
   :scale: 50%
   :alt: Order Panel (Data format)
   :align: center

   Order Panel (Data format)

Make your choice and click on "**Next**". This brings you to the next tab of the Order Panel.
Here you can select the bands that shall be included in the product (see also :ref:`prod_guide`).
Apart from the surface reflectance bands, additional bands can be selected under "**Advanced Settings**" (see :numref:`orderPanelBands`).

.. _orderPanelBands:
.. figure:: images/OrderPanelBands.png
   :name: orderPanelBandsName
   :scale: 50%
   :alt: Order Panel (Band selection)
   :align: center

   Order Panel (Bands)

Click on "**Next**". The next page is used to assign a name to your specific order (:numref:`orderPanelOrder`).
Assign the name in such a way that it is as meaningful as possible. This way you will be able to distinguish your processings better later on.

.. _orderPanelOrder:
.. figure:: images/OrderPanelOrder.png
   :name: orderPanelOrderName
   :scale: 50%
   :alt: Order Panel (Order information)
   :align: center

   Order Panel (Order information)

Note that large orders might be split into several tiles. The Sentinel tile names will appear as subfolders in the
product when downloaded.

Click on "**Next**". You will get to the last page (see :numref:`orderPanelConfirmOrder`).
As mentioned before, you are now able to review your decisions and make changes if necessary.

.. _orderPanelConfirmOrder:
.. figure:: images/OrderPanelConfirmOrder.png
   :name: orderPanelConfirmOrderName
   :scale: 50%
   :alt: Order Panel (Confirm Order)
   :align: center

   Order Panel (Confirm Order)

If everything is correct, click on "**Generate**". The processing starts and after a while (depending on the size of the order)
you will be able to download your products in the :ref:`userArea`.

.. note::
   In case your order will include more than 1 million m², product size will be very large and processing time may
   be considerable. In this case, we will get in touch with you in order identify the best way of production scheduling and
   product distribution.

.. _time_series:

Time Series
***********

The definition of a time series is very similar to the definition of a mosaic.
A click on the button "**Time Series**" brings up the following page (see :numref:`timeSeriesDialog`):

.. _timeSeriesDialog:
.. figure:: images/TimeSeriesDialog.png
   :name: TimeSeriesDialogName
   :scale: 50%
   :alt: Time Series Dialog Page
   :align: center

   Time Series Dialog Page

Fill out all sections of the dialog and select the target pixel(s) on the map. Klicking on the lower symbol toggles
between single pixel and 3x3 pixels in the particular resolution (:numref:`timeSeriesPixels`). When done, click on "**Generate**".

.. _timeSeriesPixels:
.. figure:: images/TimeSeriesPixels.png
   :name: TimeSeriesPixelsName
   :scale: 100%
   :alt: Time Series Pixels
   :align: center

   Time Series Pixels

Successful processing changes the "Generate" button into the following message (:numref:`timeSeriesGenerated`):

.. _timeSeriesGenerated:
.. figure:: images/TimeSeriesGenerated.png
   :name: TimeSeriesGeneratedName
   :scale: 100%
   :alt: Time Series Generated Message
   :align: center

   Time Series Generated Message

Additionally, the pixels marked in :numref:`timeSeriesPixels` get a green border. Hovering over pixels will quickly display
their values and metadata; clicking on pixels will display the values on a page with the option to export data to a CSV file (:numref:`timeSeriesData`).

.. _timeSeriesHover:
.. figure:: images/TimeSeriesHover.png
   :name: TimeSeriesHoverName
   :scale: 50%
   :alt: Time Series Hover Display
   :align: center

   Time Series Hover Display



.. _timeSeriesData:
.. figure:: images/TimeSeriesData.png
   :name: TimeSeriesDataName
   :scale: 50%
   :alt: Time Series Data
   :align: center

   Time Series Data

.. _userArea:

User Area (Download)
********************

Clicking on the button "**User Area**" in the Mosaic Hub App brings up the following dialog window (:numref:`userAreaImage`):

.. _userAreaImage:
.. figure:: images/UserAreaImage.png
   :name: userAreaImageName
   :scale: 50%
   :alt: User Area
   :align: center

   User Area

The User Area is the place where you can download your products after completion of the production. The user area also
allows you to monitor and cancel your orders during production or get in touch with the S2GM team in case of issues.
After completion of a production, your products will be available for a period of 2 weeks for download.
The User Area displays all current mosaic orders. You are able to filter for a production name to narrow your search.
If something went wrong, you can inform the S2GM team by clicking on the envelope icon. Orders can be cancelled by clicking
on the red cross icon. If the status of an order is finished, the download icon changes to green. When you click on it,
the download dialog will be displayed (:numref:`mosaicDownloaderList`). You first have to select a download directory
that you can change later if needed.
Hovering the list will turn the entries from grey to black. A click on the black icon will start the download.

.. _mosaicDownloaderList:
.. figure:: images/MosaicDownloaderList.png
   :name: mosaicDownloaderListName
   :scale: 50%
   :alt: Mosaic Downloader List
   :align: center

   Mosaic Downloader List

As already mentioned above: if you selected a large area, the orders might be split into several tiles that appear in the
download list after you clicked on the download button. To avoid unnecessary processing in the Mosaic Hub,
processings and thus the downloads will proceed only after user involvement. Also, you will be notified that more tiles
might be available (:numref:`moreTiles`). The red check mark signifies that the download is not yet complete.

.. _moreTiles:
.. figure:: images/MoreTiles.png
   :name: moreTilesName
   :scale: 50%
   :alt: More Tiles available
   :align: center

   More Tiles available

The following image shows an example download directory for a multi-tile product:

.. _tilesDownloaded:
.. figure:: images/TilesDownloaded.png
   :name: tilesDownloadedName
   :scale: 50%
   :alt: Tiles downloaded to the file system
   :align: center

   Tiles downloaded to the file system



