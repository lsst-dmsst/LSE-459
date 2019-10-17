.. image:: https://img.shields.io/badge/dmtn--134-lsst.io-brightgreen.svg
   :target: https://dmtn-134.lsst.io
.. image:: https://travis-ci.com/lsst-dm/dmtn-134.svg
   :target: https://travis-ci.com/lsst-dm/dmtn-134

##########################################################
Expectations and questions while interacting with DOE labs
##########################################################

DMTN-134
========

SLAC, Fermilab and Brookhaven National Laboratory have been requested to look into supporting LSST computing during the operational era.
This note is to help both sides in the process of establishing what this means and how LSST can evaluate it.

Links
=====

- Live drafts: https://dmtn-134.lsst.io
- GitHub: https://github.com/lsst-dm/dmtn-134

Build
=====

This repository includes lsst-texmf_ as a Git submodule.
Clone this repository::

    git clone --recurse-submodules https://github.com/lsst-dm/dmtn-134

Compile the PDF::

    make

Clean built files::

    make clean

Updating lsst-texmf
-------------------

`lsst-texmf`_ includes BibTeX files, the ``lsstdoc`` class file, and acronym definitions, among other essential tooling for LSST's LaTeX documentation projects.
To update to a newer version of `lsst-texmf`_, you can update the submodule in this repository::

   git submodule update --init --recursive

Commit, then push, the updated submodule.

.. _lsst-texmf: https://github.com/lsst/lsst-texmf
