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


