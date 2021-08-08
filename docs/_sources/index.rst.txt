.. flintyPy documentation master file, created by
   sphinx-quickstart on Wed Aug  4 08:28:41 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

**flintyPy**
====================================

This is the homepage of **flintyPy**, the Python version of the software **flinty** (Flexible and Interpretable Non-parametric Tests of Exchangeability). The R version is available `here <https://alanaw1.github.io/flintyR>`_. 

What does this package offer?
-----------------------------

**flintyPy** provides exact tests of exchangeability in multivariate datasets.

- It is *non-parametric* (i.e., makes no distributional assumptions of the features), which makes it suitable for settings where the user might prefer not to make distributional assumptions about their data.
- It is *flexible*, meaning that the practitioner can specify feature dependencies based on their knowledge of the problem, or can simply provide summary statistics in the form of pairwise distance data. See Examples for details.
- It is *scalable*, so the user does not have to worry about the sample size :math:`N` or the number of features :math:`P` of the data.
- It is *robust*, meaning that it controls for false positive rate (FPR) and remains powerful in realistic settings including uneven representation of subpopulations, sparsity of discriminative features, and small sample sizes.

How to install?
---------------

**flintyPy** requires Python >= 3.7.10, and for now we recommend the following installation procedure that uses both ``conda`` and ``pip``. 

1. Download `anaconda <https://www.anaconda.com/download/>`_ or `miniconda <https://conda.io/miniconda.html>`_. 
2. Create a separate conda environment and install some required packages.

.. code-block:: console

    conda create -n flinty python==3.7.10
    conda activate flinty
    conda install numpy==1.21.1
    conda install numba==0.53.1
    conda install scipy==1.7.1

3. Install **flintyPy** (v0.1.17, on Test PyPI) using pip. 

.. code-block:: console

    pip install -i https://test.pypi.org/simple/ flintypy==0.1.17

For guidance on running our exchangeability test, please click on the "Examples" tab.

API reference
------------------

Our :ref:`flintypy` contains detailed descriptions of the main and auxiliary functions.

Indices
-------

* :ref:`genindex`
* :ref:`search`