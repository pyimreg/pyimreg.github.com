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
* <a href='#dipy'>dipy</a>
* <a href='#antspy'>ANTsPy</a>
* <a href='#nireg'>nireg</a>
* <a href='#simpleelastix'>SimpleElastix</a>
* <a href='#pirt'>PIRT</a>
* <a href='#python-register'>Python-register</a>
* <a href='#silx'>Silx</a>
* <a href='#gefolki'>GeFolki</a>

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


### dipy

[Dipy](http://nipy.org/dipy/) includes methods for Diffeomorphic registration in
[2D](http://nipy.org/dipy/examples_built/syn_registration_2d.html)
and [3D](http://nipy.org/dipy/examples_built/syn_registration_3d.html).

Installation: see [instructions](http://nipy.org/dipy/installation.html)

### nireg

[nireg](https://github.com/nipy/nireg) aims to be a dedicated pure-Python image registration package. 

It is yet to be fully documented and made usable to dummy users.

### ANTsPy

[ANTsPy](https://github.com/ANTsX/ANTsPy) is a Python library which wraps the C++ biomedical image processing library ANTs, which has registration capabilities. Some documentation is available, and it is yet to be fully documented.


### SimpleElastix

[SimpleElastix](https://simpleelastix.github.io/) is an extension of SimpleITK
that includes Elastix to offer more registration algorithms.

Installation: compilation is difficult, but there is an
[effort](https://github.com/conda-forge/staged-recipes/pull/324) to put it
on conda-forge.


### PIRT

[PIRT](http://pirt.readthedocs.io) is a framework for exposing
a variety of elastic registration algorithms via a common API, including
Demons, a diffeomorphic (i.e. geometrically correct) variety of  Demons, and
more. The algorithms were previously written in Cython, but are now implemented
in Python, yet running at C-speed thanks to Numba, making installation easy.
Not very actively maintained at the moment.

Installation: pip


### Python-register

[python-register](https://github.com/pyimreg/python-register) is a package
for image registration built on top of scipy and numpy.

Installation: needs compilation


### Silx

The [Silx toolkit](https://github.com/silx-kit/silx) includes a GPU-based
SIFT registration algorithm.

Installation: needs compilation?

### GeFolki

[GeFolki](https://github.com/aplyer/gefolki) (Geoscience Extended FlOw Lucas- Kanade Iterative) is a coregistration method that has been developped in the framework of the [MEDUSA project](https://w3.onera.fr/medusa/gefolki), first for SAR/SAR co-registration, then for other cases of remote sensing image coregistration, including hetergeneous image co-registration (ex LIDAR/SAR, optics/SAR, hyperspectral/optics and so on). It is an adaptation of an optical flow method. The method is implemented in both Python and MATLAB.

Installation: Just download the repo. Examples on how to use the modules are given. 
