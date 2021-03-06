.. _development-dependencies:

Build Dependencies
==================

.. sectionauthor:: Axel Huebl

``openPMD-api`` depends on a series of third-party libraries.
These are currently:

Required
--------

* CMake 3.10.0+
* Boost 1.62.0+: ``filesystem``, ``system``, ``unit_test_framework``

Optional: I/O backends
----------------------

* HDF5 1.8.6+
* ADIOS 1.10+ (*not yet implemented*)
* ADIOS 2.1+ (*not yet implemented*)

while those can be build either with or without:

* MPI 2.3+, e.g. OpenMPI or MPICH2

Optional: language bindings
---------------------------

* Python: (*not yet implemented*)

  * pybind11 2.3.0+
  * xtensor-python 0.17.0+
