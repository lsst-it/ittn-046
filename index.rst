..
  Technote content.

  See https://developer.lsst.io/restructuredtext/style.html
  for a guide to reStructuredText writing.

  Do not put the title, authors or other metadata in this document;
  those are automatically added.

  Use the following syntax for sections:

  Sections
  ========

  and

  Subsections
  -----------

  and

  Subsubsections
  ^^^^^^^^^^^^^^

  To add images, add the image file (png, svg or jpeg preferred) to the
  _static/ directory. The reST syntax for adding the image is

  .. figure:: /_static/filename.ext
     :name: fig-label

     Caption text.

   Run: ``make html`` and ``open _build/html/index.html`` to preview your work.
   See the README at https://github.com/lsst-sqre/lsst-technote-bootstrap or
   this repo's README for more info.

   Feel free to delete this instructional comment.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. TODO: Delete the note below before merging new content to the master branch.

.. note::

   **This technote is not yet published.**

   Information regarding the installation of MTP / MPO fiber optics for the third floor

.. Add content here.

INTRODUCTION
=============

The following documentation provides a closer look at MTP / MPO fiber connections from the second floor to the third floor, while also providing an inside look at the materials 
used and the areas involved. The Rubin IT Team is in charge of installing the MTP / MPO fiber optic cable that originates from the computer room located on the second floor of 
the main building and extends to the staging area outside the cleanroom and room. clean on the third floor.


The IT requirements are the following:

- Install the 13 cables from the second floor to the third floor of the main building.
- Separate 12 of those cables for the DAQ connections and use one of those cables for the CCS

The cables used for this project were OM3/OM4 with 24 filaments MTP/MPO connectors with type A polarity. It is important to mention that both the OM3 and OM4 cables are fully
compatible with each other. The specifications for this setup were provided by the National Accelerator Laboratory Group (SLAC). To know more about this please visit the 
following sources:  RM-2010 / LSE-65 / IT-1384.

- https://jira.lsstcorp.org/browse/RM-2010
- https://docushare.lsst.org/docushare/dsweb/Get/LSE-65
- https://jira.lsstcorp.org/browse/IT-1384?jql=text%20~%20%22DAQ%22


Technical Specifications for the materials used
================================================

Cable Jacket
------------

Due to the geographical location of the telescope and weather conditions, it was decided to install The OFNP cables that have the highest fire rating, suited for vertical runs 
between floors in data centers.

.. figure:: /_static/1.jpg
   :name: 1
   :width: 700 px

Image: Prototype of the Armored Cable

Additional Technical Specifications:

.. figure:: /_static/2.PNG
   :name: 1
   :width: 700 px
   
MTP / MPO connectors and adapters
---------------------------------
MTP/MPO main characteristics and features

MTP/MPO Connector
^^^^^^^^^^^^^^^^^^
Each cable contains 24 filaments with 1 MTP/MPO connector at each end.

.. figure:: /_static/3.jpg
   :name: 1
   :width: 700 px
   
   Image: MTP/MPO Connectors
   
   MTP/MPO Adapters
   ^^^^^^^^^^^^^^^^

Each connection between cables has to use a key-up and key-down adapter in order to work and function properly.

.. figure:: /_static/4.jpg
   :name: 1
   :width: 700 px
   
Image: Key-up and Key-down adapter.

The MTP / MPO Female and Male Connectors
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The MTP/MPO cables always connect to another MTP/MPO cable, each connector has a connection type which is either Female or Male.

.. figure:: /_static/5.jpg
   :name: 1
   :width: 700 px
   
Image: MTP/MPO Connectors Female/Male


Cable Polarity
--------------

The cable can be purchased in 3 polarity modes, these are:

- Type A
- Type B
- Type C

For documentation purposes, we will turn our focus on Polarity Type-A cables.

.. figure:: /_static/6.jpg
   :name: 1
   :width: 700 px
   
   .. figure:: /_static/7.jpg
   :name: 1
   :width: 700 px

Image: Type A Straight Through Cable


Adapter Keys
------------

When we refer to the adapter key, it is a notch in the coupler that gives the connection orientation of the connectors. The polarities that are compatible with these adapters
are Type A and Type B.

- A Type A adapter or coupler polarity is (Key Up to Key Down)

- A Type B adapter or coupler polarity is  (Key Up to Key Up)

In this report, we will only document the Type A coupler.

 .. figure:: /_static/8.jpg
   :name: 1
   :width: 700 px

Cable Connection Method
-----------------------

To connect these cables we will need to use the corresponding adapter for the polarity of the cable used. The image below illustrates the connection method used for a male-to-
female type A cable using a coupler with Flange (Key Up to Down).

 .. figure:: /_static/9.jpg
   :name: 1
   :width: 700 px

MTP / MPO cable acquisition method
===================================

Our MTP/MPO cables are supplied by a factory that specializes in fiber optic materials and structured cabling. We have been working with this company throughout the construction
period of the telescope at Rubin, providing us with network cables, fiber optic cables, specific tools, and any other material related to structured cabling. One of the
advantages that we have working with this company is that we have direct contact with a representative allowing us to place special orders or requests for a specific type of
material we would like to work with satisfying our needs.

Purchase Method
---------------

To purchase a specific cable we need to know the type of cable we would like to use, its polarity, and any other feature required. Once all of this information is gathered a
company representative is contacted with our requirements and the order is received and processed. The company then proceed to manufacture the cable and Is shipped to Tucson and
later to Chile which is received by the IT Team at the AURA Facility all in approximately 2 months.














.. Do not include the document title (it's automatically added from metadata.yaml).

.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
