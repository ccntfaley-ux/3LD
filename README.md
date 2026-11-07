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

