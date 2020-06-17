{% set name = "fermitools-run-deps" %}
{% set version = "1.0" %}

package:
  name: {{ name|lower }}
  version: {{ version }}

build:
  number: {{ environ.get('BUILD_NUMBER', 0)}}

requirements:
  run:
    - ape >=3
    - aplpy
    - astropy
    - blas
    - clhep
    - cppunit
    - f2c 0.0.2.*
    - fermitools-data
    - fftw
    - gsl
    - healpix_cxx
    - matplotlib
    - numpy >=1.11
    - pmw
    - python 2.7
    - pyyaml
    - root >=6.0
    - scipy
    - wcslib <6
    - xerces-c
