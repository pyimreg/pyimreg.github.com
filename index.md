# List of (non-rigid) image registration projects for Python


## Purpose

This is a curated list of Python projects for non-rigid (i.e. elastic)
image registration. Currently, there is not a single library that stands
out as *the* way to do image registration. This is in part because image
registration is hard and there is a large variety of methods which is
perhaps difficult to collect in a single library. But this is also
because there has not been a collaborative effort to make such a
library.

This website is a small step in unifying efforts related to image
registration in Python by providing a single place to list the current
projects and their status. It should give users who need tools for
registration problems a better idea of what library they could best
use. Further, developers who want to implement new tools have a better
idea of what's already out there, and what other developers they might
collaborate with.


## Contributing

If you know of a library/project that's not listed here, or think that
the information on this page is inaccurate, please help improve this
site by making a contribution via
[the Github page](https://github.com/pyimreg/pyimreg.github.com).


## The list

* <a href='#scikit-image'>Scikit-Image</a>
* <a href='#simpleitk'>SimpleITK</a>
* <a href='#pyelastix'>PyElastix</a>
* <a href='#nipy'>Nipy</a>
* <a href='#simpleElastix'>SimpleElastix</a>
* <a href='#pirt'>PIRT</a>
* <a href='#python-register'>Python-register</a>
* <a href='#silx'>Silx</a>


----

### Scikit-Image

[Scikit-Image](http://scikit-image.org) is a popular and well-maintained image processing toolkit,
which also provides a
[framework](http://scikit-image.org/docs/stable/api/skimage.transform.html)
for finding the transform between images and using it to
[warp](http://scikit-image.org/docs/stable/api/skimage.transform.html#warp)
one image onto another.

Installation: available via conda.


### SimpleITK

[SimpleITK](https://github.com/SimpleITK/SimpleITK) is a C++ library
that has bindings for Python. See e.g. examples for
[B-spline](https://github.com/SimpleITK/SimpleITK/blob/next/Examples/ImageRegistrationMethodBSpline1/ImageRegistrationMethodBSpline1.py)
and [Demons](https://github.com/SimpleITK/SimpleITK/blob/next/Examples/DemonsRegistration1/DemonsRegistration1.py).

Installation: via [conda](https://anaconda.org/SimpleITK/simpleitk) or
[pip](https://pypi.python.org/pypi/SimpleITK).


### PyElastix

[PyElastix](https://github.com/almarklein/pyelastix) is a thin wrapper around
the Elastix toolkit. Written in pure Python, so no compilation required.

Installation: pip or conda.


### Nipy

[Dipy](http://nipy.org/dipy/) includes methods for Diffeomorphic registration in
[2D](http://nipy.org/dipy/examples_built/syn_registration_2d.html)
and [3D](http://nipy.org/dipy/examples_built/syn_registration_3d.html).

The nireg subopackage also provides functionality image registration.
Need more info.

Installation: see [instructions](http://nipy.org/nipy/users/installation.html)


### SimpleElastix

[SimpleElastix](https://simpleelastix.github.io/) is an extension of SimpleITK
that includes Elastix to offer more registration algorithms.

Installation: compilation is difficult, but there is an
[effort](https://github.com/conda-forge/staged-recipes/pull/324) to put it
on conda-forge.


### PIRT

[PIRT](https://bitbucket.org/almarklein/pirt) is a framework for exposing
a variety of elastic registration algorithms via a common API, including
Demons, a diffeomorphic (i.e. geometrically correct) variety of  Demons, and
more. The algorithms are written in Cython for speed, and therefore needs
compilation. It's a bit idiosyncratic, tied to visvis, and the original
developer does not have time to maintain it mutch.

Installation: needs compilation


### Python-register

[python-register](https://github.com/pyimreg/python-register) is a package
for image registration built on top of scipy and numpy.

Installation: needs compilation


### Silx

The [Silx toolkit](https://github.com/silx-kit/silx) includes a GPU-based
SIFT registration algorithm.

Installation: needs compilation?

