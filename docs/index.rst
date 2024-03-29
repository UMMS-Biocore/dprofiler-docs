.. Dprofiler documentation master file, created by
   sphinx-quickstart on Tue Sep 13 14:28:12 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Dprofiler's documentation!
=====================================

What is Dprofiler ?

Biospecimen collected from multiple sources of experimental and technical conditions often exhibit **diverse molecular profiles and patterns**. Each individual sample presents an additional source of information towards elucidating biological mechanisms, and each sample may even be more informative than the differential expression between phenotypic conditions

Understanding complex patterns of expression profiles are essential to solving diseases, and such knowledge can only be generated by using advanced statistical measures and methods that are capable of computationally modeling and **separately investigating molecular profiles of each sample**.

To deciphering these complex molecular profiles within gene expression datasets, we have developed **Dprofiler**.

.. image:: /dprofiler_pics2/DprofilerWorkflow.png
  :align: center
  :width: 60%

This application computationally profiles a set of targeted samples by connecting them to reference expression datasets with phenotypic profiles of interest. Building on these reference profiles of phenotypic groups, Dprofiler evaluates bulk RNA samples, detect possibly existing anomalies and heterogeneities, and further explores causes and sources of distinct molecular patterns with the aid of single cell maps and other reference gene expression datasets.

Users are allowed to use a variety of algorithms to calculate a **Membership Score** of samples associated to some phenotypic profiles of interest. Dprofiler derives reference phenotypic profiles from submitted datasets, cell-types of single cell maps and conditions from external gene expression data sets. Membership scores are universally interpretable, and indicate the similarity of a sample to these reference profiles.

Dprofiler offers multiple capabilities using these three components:

* **Computational Profiling**: Scoring and Profiling submitted samples using homogeneouos subpopulations of phenotypic reference profiles within the same dataset.
* **Cellular Composition Analysis**: Infering the cellular composition of each scored sample with a reference scRNA data and estimate fractions of cellular compositions.
* **Comparative Profiling**: Scoring and Profiling samples using targeted phenotypic profiles of a reference bulk expression data set.
Dprofiler is based on a recently developed Shiny (R) application, DEBrowser, an interactive tool for DE analysis and visualization. DEBrowser incorporates DESeq2, EdgeR, and Limma coupled with shiny to produce real-time changes within your plot queries and allows for interactive browsing of your DE results. DEBrowser also manipulates your results in a way that allows for interactive plotting by which changing padj or fold change limits also changes the displayed graph(s).

Contents:

.. toctree::
   :maxdepth: 2

   quickstart/quickstart
   diffhetero/diffhetero
   cellcomp/cellcomp
   compprof/compprof
   deseq/deseq
   references/references
