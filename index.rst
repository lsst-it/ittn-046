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

.. figure:: /_static/1
    :name: 1
    :target: 700px

Image: Prototype of the Armored Cable


.. Do not include the document title (it's automatically added from metadata.yaml).

.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
