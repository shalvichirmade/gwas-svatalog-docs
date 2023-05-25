.. GWAS SVatalog documentation master file, created by
   sphinx-quickstart on Tue Feb 28 13:36:49 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. figure:: gwas-svatalog-name.svg
   :target: index.html
   :width: 400px
   :alt: logo




Welcome to GWAS SVatalog's documentation!
=========================================

**GWAS SVatalog** is a web tool that allows the user to visualize structural variants (SVs) and single nucleotide polymorphisms (SNPs) in high linkage disequilibrium (LD). The software is availible here (insert link to tool).

.. note::

   This project is under active development.


Filters
-------

The filters are used to subset the SVs based on the chosen criteria. There are three ways to accomplish this:

* **Gene**: select chromosome and/or gene of interest.

  * The SVs displayed are within 100kb of the start and end of the gene chosen.

* **Genomic Region**: select chromosome and/or base pair range.

  * The SVs displayed are within the region chosen.

* **Phenotype**: select phenotype of interest depicted in the GWAS Catalog database.

  * If the SNP associated with this phenotype has linkage disequilibrium inforamtion with an SV, these SVs will be displayed. If a phenotype is chosen along with the gene or genomic region filter, both criteria will be used to subset the SV list.

..
   Add image of filter section here


SV Table
--------

The default table contains all the SVs identified in *Homo sapiens*, as described in (insert citation to paper). The table will automatically update based on the filters selected, as explained in `Filters`_.

The user will need to select an SV of interest to generate the interactive plot showcasing the SNPs in LD.

..
   Add image of SV table section here


Annotation Table
----------------

Based on the SV selected in `SV Table`_, this table will display the corresponding annotations for the SV region. :doc:`This document <annotation>` explains the meaning of each column in detail.

..
   Add image of annotation table section here


SV-SNP Colocalization Plot
-------------------------------

This plot shows the colocalization between SNPs and a single SV. It will autopopulate when a SV is chosen from the SV table. 

There are two main ways the visualization can be displayed:

1. Selection of phenotype:

   * The plot will be against the p-value found in the GWAS Catalog.
   * The plot will display all SNPs in the GWAS Catalog and highlight the SNPs in linkage with the SV and associated with the phenotype chosen.
   * The SNPs will be highlighted based on the R\ :sup:`2` linkage value with the SV selected.
   * The size of the highted SNPs will be based on the D' linkage value with the SV selected.

..
   Add image of plot type here


2. Without the selection of phenotype:

   * The plot will be against the R\ :sup:`2` linkage value with the SV selected.
   * The plot will display all SNPs available in the linkage dataset.
   * The SNPs will be sized based on the D' linkage value.
   * The SNPs in blue are also found in GWAS catalog while the SNPs in black are not.

..
   Add image of plot type here



.. toctree::
   :maxdepth: 2
   :caption: Contents:
   index
   annotation




.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`

