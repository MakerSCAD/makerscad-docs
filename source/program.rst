.. _programming:

##########################
  Programming tools
##########################

MakersCAD provides with some programming tools blocks, they will help you create automate and define your objects parameters.

.. _logic:

################
Logic Blocks
################

In programming logic, is very useful to compare values of variables, MakerSCAD has Comparison operators to help with these tasks
the first block is the "If" statement that allows us to compare between two variables, or compare if a variable has an specific value, or even if it is null or empty.

.. figure:: /_static/images/logic/if.png

we can help us with another blocks, like the comparator block, that will be used to determine if a variable is equal, not equal, bigger than or smaller than another variable.

.. figure:: /_static/images/logic/comparator.png

also there is a boolean logic operator block, it is used to use two conditions inside one single comparation "if" block, it has a dropdown list where you cn select "and" or "or" agregatio functions

.. figure:: /_static/images/logic/and_or.png

There is also a "test" block, best known in progrmming as the "ternary operator", it makes in a single line the comparisson between vriables using the if statement and an "else condition", executed when the main condition is not true.
in the generated code yu can see that instead of "if" and "else" words it uses "?" and ":" simbols respectively

.. figure:: /_static/images/logic/ternary.png

.. _loops:

###############
Loop Blocks
###############

.. repeatn_:

Repeat N times
================

You can use this block to make a loop in a known number of iterations, in the block you will see a text box that has a default value of ten, you can modify this value to the number of times you want the loop to be executed.

Lets make the example of the image above:

.. figure:: /_static/images/loops/repeat_n.png

First, go to "Loops" and add a "Repeat n times" block, modify the value to 3.

Now go to CAD - Scene, and bring an "Add" block, snap a Translate block to it (CAD - Transform -Translate), look at the X Y Z control, here we can put values, but also we can use programming expressions, we will put a formula in x to have each cube separated by 10 units from the others, (the size of each cube is 100), note in the generated code that there is a variable called "count" that begins with 0 and increments by 1 on each iteration, if we put "count*110" we are saying that the first cube, will have an x position of 0 * 110 = 0, the second is 110*1 = 110 and the third one is 110*2 = 220

Now, you will have 3 cubes in the workspace separated to each other by 10.

.. figure:: /_static/images/loops/for_n_example.png


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

.. figure:: /_static/images/loops/countfromto.png

.. foreachitem_:

For each item in a list
==========================

.. figure:: /_static/images/loops/foreachitem.png

.. foreachkey_:

For each key in a map
=======================

.. figure:: /_static/images/loops/foreachkey.png


.. break_:

Break out of a loop
======================

.. figure:: /_static/images/loops/break.png

.. _math:

Math Blocks
=============================

.. _text:

Text Blocks
=============================

.. _lists:

List Blocks
=============================

.. _maps:

Map Blocks
=============================

.. _color:

Color Blocks
=============================

.. _variables:

Variable Blocks
=============================

.. _functions:

Function Blocks
=============================

.. _advancedjs:

AdvancedJS Blocks
=============================
