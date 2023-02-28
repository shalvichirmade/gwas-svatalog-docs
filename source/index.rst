.. GWAS SVatalog documentation master file, created by
   sphinx-quickstart on Tue Feb 28 13:36:49 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to GWAS SVatalog's documentation!
=========================================

**GWAS SVatalog** is a web tool that allows the user to visualize the colocalization of structural variants (SVs) and single nucleotide polymorphisms(SNPs).

There are two main ways the visualization can be displayed:

1. Selection of phenotype

   * The plot will be against the p-value found in the GWAS Catalog.
   * The plot will display all SNPs in the GWAS Catalog and highlight the SNPs associated with the phenotype chosen.
   * The SNPs will be highlighted based on the R\ :sup:`2` colocalization value with the SV selected.
   * The size of the highted SNPs will be based on the D' colocalization value with the SV selected.


2. Without the selection of phenotype:

* The plot will be against the R\ :sup:`2` colocalization value with the SV selected.

* The plot will display all SNPs available in the colocalization dataset.

* The SNPs will be sized based on the D' colocalization value.

* The SNPs in blue are also found in GWAS catalog while the SNPs in black are not.


.. note::

   This project is under active development.


.. toctree::
   :maxdepth: 2
   :caption: Contents:



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
