# DynamicalBilliards

C++ program that allows the user to create any straight-line dynamical-billiard geometry and subsequently simulate an arbitrary number of boundary collisions from an arbitrary starting point.

Program asks user to specify the start and end points of all lines in the geometry using a standard Cartesian coordinate system (x being "horizontal", and y "vertical"). There are no restrictions on the specification of the lines. The starting point for the particle must then be specified, along with a direction in the form of a two-component vector. Again, there are no restrictions on these two things; more specifically, the former may be placed anywhere, even outside a closed geometry if desired.

Finally, the number of iterations (boundary collisions/reflections) must be specified. If your setup is such that the particle makes no further boundary collisions before your chosen number of iterations, the program will terminate early. As an example, consider a straight-line geometry from (0,0) to (0,2), and a particle fired from (-1,0) with direction vector (1,1): the particle will reflect from the geometry at (0,1), and the program will subsequently terminate, no matter the number of iterations set.

All the collision/reflection points are recorded, along with the iteration number, in a .txt file.

The zip contains three files; "main1.cpp" is the one to compile.
