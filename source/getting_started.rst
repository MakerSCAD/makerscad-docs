.. _getting_started:


***************
Getting started
***************

.. _opening:

Opening MakersCAD
=============================

First go ahead and visit `MakersCAD <http://MakersCAD.com/>`_
remember this is an early Alpha testing version expect the following things to happen:

* Things might break.
* Current version might lose compatibility with future versions.
* Chrome and Chrominium web browsers are supported for now.
* MakersCAD and its documentation are under heavy development things will change!

If you find any bugs and want to help us out send us an email at::

  info@MakersCAD.com

.. _interface:

The MakersCAD interface
=============================

.. figure:: /_static/images/gettingstarted/ui.png

    The MakersCAD UI

First, we have the main toolbar

.. figure:: /_static/images/gettingstarted/maintoolbar.png

.. figure:: /_static/images/gettingstarted/maintoolbar1.png


   the main toolbar

Here you can:

* SAVE your current work, it overwrites the latest save state.
* LOAD the latest saved version
* EXPORT your work into an xml file, for now the is test.xml increasing the file number, for example test1.xml,test2.xml... finding the next available number.
* EXPORT the current 3d objects as a STL file.
* EXPORT the current 3d objects as an OBJ file.
* LOAD an asset (experimental).
* Confifure MakersCAD on the SETTINGS window.
* Go to the Documentation to get HELP learning MakersCAD
* Check the ABOUT window for authors, copyright licence and more.

Under the main toolbar at the left side is Work view

.. figure:: /_static/images/gettingstarted/workview.png

Here we have the block library.

.. figure:: /_static/images/gettingstarted/library.png

    The block library

* :ref:`cad`, Special blocks related to shapes, objects and parts.
* Logic
* Loops
* Math
* Text
* Lists
* Color
* Variables
* Functions
* Library

and the block workspace where we will be creating our 3D world.

.. figure:: /_static/images/gettingstarted/workspace.png

    The block workspace


Some useful controls for our block workspace:

* Pan the view up, down, right and left::

      Right click + Drag

* Zoom in and Out::

      Mouse wheel up or down


On the Left side at the the top theres our 3D view, where we can se a preview of our world.

.. figure:: /_static/images/gettingstarted/3dview.png

      The 3D view.

Here you are able to:

* look around your current object in 3D::

      Right click + Drag

* Pan the camera up, down, right and left::

      Shift + Right click + Drag

      or

      MMB + Drag

* Zoom in and Out::

      Mouse wheel up or down

      or

      Ctrl  + Right click + Drag

Under the 3D view theres a javascript viewer that allows us to view and debug the code created from our blocks to display our 3D world.

.. figure:: /_static/images/gettingstarted/jsviewer.png

    The Javascript code viewer

Finally at the bottom its our Draw Toolbar, here we can turn on and off the automatic update to see in realtime the changes we are making on our blocks, manually update and DRAW the 3D View or PLAY our world in a new window.

.. figure:: /_static/images/gettingstarted/draw.png

    The draw toolbar
