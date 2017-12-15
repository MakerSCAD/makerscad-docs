.. _loops:

###############
Loop
###############

.. repeatn_:

Repeat N times
================

You can use this block to make a loop in a known number of iterations, in the block you will see a text box that has a default value of ten, you can modify this value to the number of times you want the loop to be executed.

Lets make the example of the image above:

.. figure:: /_static/images/loops/for_n_example.png

First, go to "Loops" and add a "Repeat n times" block, modify the value to 3.

Now go to CAD - Scene, and bring an "Add" block, snap a Translate block to it (CAD - Transform -Translate), look at the X Y Z control, here we can put values, but also we can use programming expressions, we will put a formula in x to have each cube separated by 10 units from the others, (the size of each cube is 100), note in the generated code that there is a variable called "count" that begins with 0 and increments by 1 on each iteration, if we put "count*110" we are saying that the first cube, will have an x position of 0 * 110 = 0, the second is 110*1 = 110 and the third one is 110*2 = 220

Now, you will have 3 cubes in the workspace separated to each other by 10.

.. figure:: /_static/images/loops/repeat_n.png

.. while_:

Repeat While
==============

When you have a condition that must be true to continue the loop, but not necessarly know the exact number of iterations you can use the while loop.

.. figure:: /_static/images/loops/repeatwhile.png

To do the last excersise using a while loop go to "Loops" and add a repeat while" block to the workspace.

.. figure:: /_static/images/loops/while_example.png

.. warning::
  Be sure that the Auto render option is not checked in when you are begining a while loop, and only click "Draw" once you have set the condition to exit the while".

The first thing you will note is that there is a dropdown menu where you can select "while" or "until" the difference is that if you select "while" the loop will continue while the condition is true, but if you select "until" the loop will continue while the condition is false, for the excersise whe will leave the "while option"

Then, go to Variables and select the block that says "Var1", snap it to the while and write the following expression ::
count < 3

The expresion says that when control variable "count" reaches the value of 3 the loop will break and will not do more iterations. If you had used "until" instead of while, the expression could had been ::
count = 3

you can also use a comparator block and var blocks to avoid writing the whole expresion


.. countfromto_:

Count From/To
================

You can set the increment and the initial value of the control variable in a for loop, for that purpose MakerSCAD has the Count From/To block.

.. figure:: /_static/images/loops/countfromto.png

we will make an excersise very similar to the one on the Repeat n Times section, but the difference is that this time variable called "count" will be called "i" (in later versions you will change the name), begins with 0, ends in 6 and will have an increment of 3 on each iteration. That way we will have the same 3 cubes, the first cube will have an x position of 0 * 110 = 0, the second is 110*3 = 330 and the third one is 110*6 = 660

Now, you will have 3 cubes in the workspace separated to each other by 230.

.. figure:: /_static/images/loops/fromtoexample.png

.. foreachitem_:

For each item in a list
==========================

In MakerSCAD there is a block to iterate between each element of a list.

.. figure:: /_static/images/loops/foreachitem.png

To do this exampple, lets create a variable for the list, go to Variables and pick a var block, name it "my_list" then go to "Lists", pick a  "Create list with" block and snap it to the variable.

look at the add sign (+) in the block click it twice to create two slots more and snap a sphere on each one, you will have now a list with 3 spheres, set each one a diameter of 40.

Now go to Loops and pick a "For each item block", snap a var1 block and write "my_list" on it, that will make the loop to iterate over each item on "my list" and will call each element "j"  

Go to CAD - Scene and píck an "Add" block, then CAD - Transform and pick a translate and use them into the loop, in the x control of the translate block write "j_index * 50" and finally add a var block to use the j variable.

your excersise should look like the picture, you will see three spheres

.. figure:: /_static/images/loops/foreachexample.png

finally 
 
.. foreachkey_:

For each key in a map
=======================

.. figure:: /_static/images/loops/foreachkey.png


.. break_:

Break out of a loop
======================

you can interrupt the excecution of a loop with a spoecial Block called break

.. figure:: /_static/images/loops/break.png

This is very useful for example when you are searching for an element in a list, you ask for the property you look for, and when you find it you can break out the loop to not continue.

the block also has an engine icon where you can change the expression from "break" to continue, the difference is that while the "break" expression interrupts the loop at all, the continue only pass by the iteration where the condition is acompplished but go immediately to the next iteration.

In the following image whe can see a list with a torus, a sphere and a cylinder, in that order, then, a loop that iterates each item in the list, and a break expresion that is excecuted if the index is 1, remember that in programming, a list or array begins with 0, so, what are we doing is to break out in the second iteration, and only the torus is added to the scene.

.. figure:: /_static/images/loops/breakexample.png

In the other hand, we have the same excersise but this time we used the continue, instead of "break", so, the loop breaks in the element with index "1" (the sphere) but continues with the next iteration and adds the element "2" (the cylinder).

.. figure:: /_static/images/loops/continueexample.png

