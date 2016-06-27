.. _cad:


***************
The CAD blocks
***************

.. _basicscene:

The basic scene
=============================

In order to start creating a 3D world we first need to set up a scene, in ScratchyCAD we have preloaded a basic scene that comes with some basic lightning, material and shadow presets.
The basic scene can be found in the block library under the CAD/Tools section.

It looks like this:

.. figure:: /_static/images/CAD/newbasicscene.png

      the basic scene block.

Go ahead and add a new basic scene to our workspace, right now it is an empty scene that we need to start adding objects to it in order to build our world.

.. _sceneadd:

Next  we have the scene.add block, this allows us to add an object to our scene objects include shapes, geometries, lights and more go ahead and take the scene.add block and plug it under the basic scene block.


.. figure:: /_static/images/CAD/sceneadd.png

      adding objects to our scene.

By default the add.scene block comes preloaded with a cube, go ahead and press the DRAW button! he have succesfully added our first object to our scene.

.. figure:: /_static/images/CAD/firstscene.png


Now that we know hot to add objects to our world lets look at some of them:

.. _box:

The Box
=============================

The box geometry is found under the CAD/parts library
Go on and grab the cube block and plug it to the scene.add block.

this is the ScratchyCAD default box that measures 100x100x100 units.

.. figure:: /_static/images/CAD/box.png

      ScratchyCAD's default box

The first parameter in the cube is asking for a size XYZ, for every parameter in ScratchyCAD
that asks for XYZ we need to plug in a special block that contains a list of three numbers
one for lenght (x), one for width (y) and one for height (z).
For now grab lets use the preset and change the values on the  x,y,z inputs. Activate the Auto checkbox on the left right corner and see how each value affects the box.

.. figure:: /_static/defaultcubelist.png

      xyz block in the Lists ibrary

.. figure:: /_static/defaultcubelist1.png

      xyz plugged to the cube block

Now we have a list we only need to get some values. Under the math library look for the first block that
contains a value of 0, this is a number block, it returns the value that the user types on it, or the variable that's connected to it.
Go ahead and grab three number blocks for each of the xyz inputs. Try different numbers out,
remember to turn un the AUTO in order to see the changes as you type.

.. figure:: /_static/cubenumber.png

      the number block.

.. figure:: /_static/cubenumber1.png

      testing values on the cube xyz input.

.. _sphere:

Using the sphere block
=============================

The sphere block can be found under the CAD/Parts library.

.. figure:: /_static/sphereblock.png

      the default sphere block.

The sphere has two parameters:
      * Diameter, a numeric value and defines the size of the sphere
      * Resolution, a numeric value that defines the number of poligons that make the shape

.. figure:: /_static/sphereblock1.png

      the sphere block

.. figure:: /_static/sphereblock1.png

      high resolution sphere

.. figure:: /_static/sphereblock1.png

      low resolution sphere

.. _cylinder:

Using the cylinder block
=============================

The cylinder block can be found under the CAD/Parts library.

.. figure:: /_static/cylinder.png

      the default cylinder block.

This block has four parameters:

      * Diameter1, a numeric value that defines the size of the lower base.
      * Diameter2, a numeric value that defines the size of the upper base.
      * Height, a numeric value that defines how tall is the cylinder.
      * Sides, a numeric value that defines how many sides our prism will have.

.. figure:: /_static/cylinder1.png

      a cylinder with equal diameters and five sides.

.. figure:: /_static/cylinder2.png

      a cylinder with larger diameter2 and eight sides.

.. figure:: /_static/cylinder3.png

      a cylinder with a larger diameter1 and eight sides.

.. figure:: /_static/pyramid.png

      a pyramid can be made with a size zero diameter2.


.. _polygon:

Using the polygon block
=============================

The polygon block defines a 2D shape, this shape is given by a list of  at least three points (x,y,z) or vertices.
This given list of vertex creates a face in the x,y plane.

Go ahead and get the polygon block from the CAD/Parts library and plug it to your main function, by default it returns a
triangle rectangle.

.. figure:: /_static/polygon.png

      the polygon block with default vertex list.

To make things easer we have included the OpenSCAD-polygon-editor that allows you to draw from scratch or trace a shape from
an image, click on the gear in the top left corner of the polygon editor.

.. figure:: /_static/polygoneditor.png

      the polygon editor interface.

From the selector menu (cursor icon) you can turn any point to a Bezier curve handle, or vertex.

.. figure:: /_static/polygonselector.png

      the polygon selector menu.

We can add new vertices by clicking on the + icon next to the selector menu.

.. figure:: /_static/addapoint.png

      add vertex.

We delete vertices by clicking on the - icon next to the + icon.

.. figure:: /_static/deleteapoint.png

      add vertex.

Finally we can add an image to trace, by setting the URL, uploading it and then scaling it..

.. figure:: /_static/traceimage.png

      trace image.

Once we are done setting up the points for our shape click close and they will be automatically added to the polygon block.


.. _text3D:


Using the text3D block
=============================

The 3Dtext block can be found under the CAD/Parts library.

It allows us to create a text based model, this block has the following main parameters:

  * text : a string value with the characters we are going to draw.
  * size: a numeric value that determines the thickness of the characters.
  * height:  a numeric value that determines the extrusion amount of the characters.

.. figure:: /_static/text3d.png

      the text3D block.


.. _part:

Using the part block
=============================

It's nice to be able to return different basic shapes, but most objects in real world are a mix
of different shapes that create a complex shape. Thats the what the Part  block is for! this one is found under the
CAD/tools library

.. figure:: /_static/ex2.png

      using the part block

The part block has three options:

* Union, adds two parts together.

.. figure:: /_static/union.png

      union of a cube with a sphere

* Difference, subtracts the second part from the first part, it's order sensitive.

.. figure:: /_static/difference.png

      difference of a cube with a sphere

.. figure:: /_static/difference1.png

      difference of a sphere with a cube

* Intersection, returns only the overlap of both shapes.

.. figure:: /_static/intersection.png

      intersection of a cube with a sphere

.. scale_:

Using the scale block
=============================

.. rotate_:

Using the rotate block
=============================

.. translate_:

Using the translate block
=============================

.. setColor_:

Using the setColor block
=============================

.. extrude_:

Using the extrude block
=============================

.. parametric_:

Making a parametric block
=============================
