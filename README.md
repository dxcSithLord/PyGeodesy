## PyGeodesy

A pure Python implementation of geodesy tools for various ellipsoidal
and spherical earth models using trigonometric and vector-based methods
for geodetic (lat-/longitude) and geocentric cartesian (x/y/z) coordinates.

Transcribed from JavaScript originals* by _Chris Veness (C) 2005-2016_
and published under the same MIT Licence*.

There are two modules for ellipsoidal earth models, _ellipsoidalVincenty_
and _-Nvector_ and two for spherical ones, _sphericalTrigonometry_ and
_-Nvector_.  Each module provides a _LatLon_ class with methods to compute
distance, initial and final bearing, intermediate points and conversions,
among other things.  For more information and further details see the
documentation*, the original JavaScript source and these geodesy descriptions:

- <http://www.movable-type.co.uk/scripts/latlong.html>
- <http://www.movable-type.co.uk/scripts/latlong-vincenty.html>
- <http://www.movable-type.co.uk/scripts/latlong-vectors.html>

Also included are modules for conversions to and from _UTM_ (Universal
Transverse Mercator) coordinates, _MGRS_ (NATO Military Grid Reference
System) and _OSGR_ (British Ordinance Survery Grid Reference) grid
references and a module for encoding and decoding _Geohashes_,
transcribed from:

- <http://www.movable-type.co.uk/scripts/latlong-utm-mgrs.html>
- <http://www.movable-type.co.uk/scripts/latlong-os-gridref.html>
- <http://www.movable-type.co.uk/scripts/geohash.html>

Two other modules provide Lambert conformal conic projections and
positions, transcribed from:

- <http://pubs.er.USGS.gov/djvu/PP/PP_1395.pdf> (John P. Snyder,
_Map Projections -- A Working Manual_, 1987, pp 107-109)

and several functions to _simplify_ or linearize a path of _LatLon_
points, including implementations of the _Ramer-Douglas-Peucker_ and
_Visvalingam-Whyatt_ algorithms and modified versions of both:

- <http://bost.ocks.org/mike/simplify/>
- <http://en.wikipedia.org/wiki/Ramer-Douglas-Peucker_algorithm>
- <http://hydra.hull.ac.uk/resources/hull:8338>

All Python source code has been statically checked* with PyChecker,
PyFlakes, PyCodeStyle (formerly Pep8) and McCabe using Python 2.7.10
or 2.7.13 and with Flake8 on Python 3.6.0 or 3.6.1.

The tests have been run with 64-bit Python 2.6.9, 2.7.13, 3.5.3 and
3.6.1, but only on MacOSX 10.10 Yosemite, MacOSX 10.11 El Capitan or
macOS 10.12.2, 10.12.3, 10.12.4 or 10.12.5 Sierra.

In addition to the PyGeodesy package, the distribution files contain the tests,
the test results and the complete documentation* generated by Epydoc.  The
```zip``` and ```tar``` distribution files were created with command line
```python setup.py sdist --formats=zip,gztar,bztar```.

Some function and method names differ from the JavaScript version.  In such
cases documentation tag ```JS name:``` shows the original JavaScript name.

__

*) Links:
 - JavaScript originals <http://github.com/chrisveness/geodesy>
 - JavaScript docs <http://www.movable-type.co.uk/scripts/js/geodesy/docs>
 - PyGeodesy package <http://pypi.python.org/pypi/PyGeodesy>
 - PyGeodesy documentation <http://pythonhosted.org/PyGeodesy>
 - MIT License <http://opensource.org/licenses/MIT>
 - PostProcessor <http://code.activestate.com/recipes/546532/>
 - PyChecker <http://pypi.python.org/pypi/pychecker>
 - PyFlakes <http://pypi.python.org/pypi/pyflakes>
 - PyCodeStyle <http://pypi.python.org/pypi/pycodestyle>
 - McCabe <http://pypi.python.org/pypi/mccabe>
 - Flake8 <http://pypi.python.org/pypi/flake8>
 - Epydoc <http://pypi.python.org/pypi/epydoc>

_Last updated: May 27, 2017._


```Copyright (C) 2016-2017 -- mrJean1 at Gmail dot com```

```Permission is hereby granted, free of charge, to any person obtaining a
copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:```

```The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.```

```THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL
THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.```
