# 3L<br>D
3Lisp,3Dimensions, a new 3d engine

3lisp OS https://3lproject.org/

Coding language https://github.com/nikitadanilov/3-lisp

to install the needed 3lisp install https://www.sbcl.org/platform-table.html and once fully installed 
download https://github.com/nikitadanilov/3-lisp/blob/master/3-lisp.cl and run
'''sbcl --load [downloaded file]''' for shell and '''sbcl --load [downloaded file] --script [file]''' for running a file


# Structure


## objects.3L
where base objects are defined and made, as well as transformations for future affine geometry support
<br>

## locator.3L
Optional file for locating where objects are
<br>

## renderer.3L
file used by interactions and standalone for rendering objects/maps, implements locator.3L if wanted
<br>


## interactions.3L
Used for running in a playable environment

# Why 3lisp?
We are using 3lisp in order to allow a truly revolutionary 3d engine. Without 3lisp our vision would be complicated and clanky. We want an engine that allows for not only the engine itself being impacted by user actions, but the actual root object to be changed, it can change the way a matrix works, it can retroactively change what has happened, it can make sure every single object is completely changed. our main application is affine geometry--with a decision you can change to what points a  line is drawn. For example in objects.3L we will use numbers on the matrix to "connect the dots" lets say you use a square ((1,0,0,0,1),(0,0,0,0,0),(0,0,0,0,0),(1,0,0,0,1)) but you may want a dip on the top so ((2,0,0,0,2),(0,1,0,1,0),(0,0,1,0,0),(3,0,0,0,3)) which with how we will encode with nearest numbers being graphed only to happened neighbors. But lets say in interactions.3L you want to change it to the highest number going to the lowest, thereby inverting the shape, or in renderer.3L changing the actual numbers, or allowing it to map to another objects points.

