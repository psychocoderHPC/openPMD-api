.. _development-buildoptions:

Build Options
=============

.. sectionauthor:: Axel Huebl

The following options can be added to the ``cmake`` call to control features.
CMake controls options with prefixed ``-D``, e.g. ``-DopenPMD_USE_MPI=OFF``:

=================== =============== ==================================
CMake Option        Values          Description
=================== =============== ==================================
openPMD_USE_MPI     **AUTO**/ON/OFF Enable MPI support
openPMD_USE_HDF5    **AUTO**/ON/OFF Enable support for HDF5
openPMD_USE_ADIOS1  **AUTO**/ON/OFF Enable support for ADIOS1 :sup:`1`
openPMD_USE_ADIOS2  AUTO/ON/**OFF** Enable support for ADIOS2 :sup:`1`
openPMD_USE_PYTHON  AUTO/ON/**OFF** Enable Python bindings :sup:`1`
=================== =============== ==================================

:sup:`1` *not yet implemented*

By default, this will build as a static library (``libopenPMD.a``) and installs also its headers.
In order to build a static library, append ``-DBUILD_SHARED_LIBS=ON`` to the ``cmake`` command.
You can only build a static or a shared library at a time.

By default, the ``Release`` version is built.
In order to build with debug symbols, pass ``-DCMAKE_BUILD_TYPE=Debug`` to your ``cmake`` command.
