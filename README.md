# Complex_Plane_Sequences

Programming Assignment 2

For this assignment we will investigate sequences in the complex plane
and determine if they are bounded or not. We will use Processing to display
a discrete portion of the complex plane. Each point in our display window
will correspond with a complex number, and each point will be put into
a recursive sequence and a method will be used to determine whether this
sequence is bounded or not. Download the file bounded seq.pde and complete
it as follows.

• Set up a display window to view the complex plane. The real axis
should extend from -3.2 to 1.6, and the imaginary axis should extend
from −1.35i to 1.35i. When calling the size() method in the setup()
method, be sure to choose values that preserve the aspect ratio.

• The variables dx and dy determine the grid that represents our discrete
space. Define these variables using the width and height keywords.

• Initialize the iterations and infinity variable. We are representing in-
finity as a finite number here.

• The for loop in the draw() method will look at each pixel on the display
window and pick its corresponding complex number. This is where you
will need your dx and dy variables. These values will represent c in the
sequence we define in the next bullet point.

• The complex sequence we are considering is recursively defined as
z<sub>n+1</sub> = z<sup>2</sup><sub>
n</sub> + c, with z<sub>0</sub> = c.

• If the current value of c results in the above sequence being bounded,
the pixel that corresponds with that value of c should be colored black.
If the sequence is not bounded, give the pixel a color that depends on
how many iterations it took to determine the sequence was unbounded.

• To decide whether a complex sequence is bounded or not, we will consider
how ‘far’ it is from the origin in the complex plane. This can be
done with the distance formula d =
&radic;<style=text-decoration:overline>&nbsp;a<sup>2</sup>&nbsp;+&nbsp;b<sup>2</sup></span>.

Since we don’t actually
need to know the Euclidean distance between a complex number and
the origin, we can remove the square root sign from the above formula
and ‘measure’ distance by the formula a
2 + b
2
.
1
Scoring Rubric
Your code compiles 1 pt
Comments and indenting 1 pt
setup() method 2 pts
Preserve aspect ratio 1 pt
Correct use of pixels[] array 2 pts
Discretization 2 pt
checkBounded() method 2 pts
Correct image displayed 1 pt
Total 12 pts
2
