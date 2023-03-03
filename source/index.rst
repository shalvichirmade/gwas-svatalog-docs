.. GWAS SVatalog documentation master file, created by
   sphinx-quickstart on Tue Feb 28 13:36:49 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. figure:: gwas-svatalog-name.svg
   :target: index.html
   :width: 500px
   :height: 350px
   :alt: logo




Welcome to GWAS SVatalog's documentation!
=========================================

**GWAS SVatalog** is a web tool that allows the user to visualize the colocalization of structural variants (SVs) and single nucleotide polymorphisms (SNPs).

.. note::

   This project is under active development.


Filters
-------

Based on the filters selected, the SV table will autopopulate to show the SVs in the chosen region.

* **Chromosome**: used to select the chromosome of interest.
* **Gene**: used to select the gene of interest.
* **Phenotype**: used to select phenotype of interest depicted in the GWAS Catalog database.

..
   Add image of filter section here


SV Table
--------

The default table contains all the SVs identified in *Homo sapiens*. The table will automatically update based on the filters selected to show the SVs in the selected regions.

The user will need to select the SV of interest to generate the colocalization plot.

..
   Add image of SV table section here


Annotation Table
----------------

Based on the SV selected above, this table will display the corresponding annotations describing this SV region. :doc:`annotationfile` explains the meaning of each column in detail.

..
   Add image of annotation table section here


SV-SNP Association Plot
-------------------------------

This plot shows the association between SNPs and a single SV. It will autopopulate when a SV is chosen from the SV table. 

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
   * The SNPs will be sized based on the D' colocalization value.
   * The SNPs in blue are also found in GWAS catalog while the SNPs in black are not.

..
   Add image of plot type here



.. toctree::
   :maxdepth: 2
   :caption: Contents:



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

