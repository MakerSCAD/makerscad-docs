.. _materials:


***************
Materials
***************

.. setColor_:

Set color
=============================

.. raw:: html

    <iframe width="560" height="315" src="https://www.youtube.com/embed/Pe1IBeBIpGE" frameborder="0" allowfullscreen></iframe>

.. setTexture_:

Set texture
=============================

.. raw:: html

    <iframe width="560" height="315" src="https://www.youtube.com/embed/mMdKvZqOPOw" frameborder="0" allowfullscreen></iframe>

.. setMaterial_:

Set material
=============================

.. basicMaterial_:

Basic material
=============================

.. lambertMaterial_:

Lambert material
=============================

.. phongMaterial_:

Phong material
=============================

.. textureLoader_:
Texture loader
=============================
Use a texture loader to load image resources as textures, to add a texture loader block go to CAD, then, Material, find the texture loader block and click it.

.. figure:: ../_static/images/CAD/textureloader.png

Once you have an object loader in your workspace, click on the gear icon to open a file selection window, if you want to load a file from your PC click the "load" button" and browse your PC for an OBJ or STL file.
Also you can enter or paste an URL in the text box and then click the "load url" button to load from a web location.


.. figure:: ../_static/images/CAD/loadassetstexture.png

you will see a preview of the file, then you can enter or click the "close" button, to close the window and go back to your workpsace


Then, to use the loaded texture you can go to CAD - Material, select a "setTexture" Block, and snap the texture loader instead of the default texture loader of the block, the result shoud look as follows:

.. figure:: ../_static/images/CAD/loadedtexture.png
