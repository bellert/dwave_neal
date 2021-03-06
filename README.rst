.. image:: https://img.shields.io/pypi/v/dwave-neal.svg
    :target: https://pypi.python.org/pypi/dwave-neal

.. image:: https://coveralls.io/repos/github/dwavesystems/dwave-neal/badge.svg?branch=master
    :target: https://coveralls.io/github/dwavesystems/dwave-neal?branch=master

.. image:: https://readthedocs.org/projects/dwave-neal/badge/?version=latest
    :target: http://dwave-neal.readthedocs.io/en/latest/?badge=latest

.. image:: https://ci.appveyor.com/api/projects/status/ihbwp21xu06h9upc/branch/master?svg=true
    :target: https://ci.appveyor.com/project/dwave-adtt/dwave-neal

.. image:: https://circleci.com/gh/dwavesystems/dwave-neal.svg?style=svg
    :target: https://circleci.com/gh/dwavesystems/dwave-neal

dwave-neal
==========

.. index-start-marker

An implementation of a simulated annealing sampler.

Example Usage
-------------

.. code-block:: python

    import neal

    sampler = neal.SimulatedAnnealingSampler()

    h = {0: -1, 1: -1}
    J = {(0, 1): -1}
    response = sampler.sample_ising(h, J)

.. index-end-marker

Installation
------------

.. installation-start-marker

To install:

.. code-block:: bash

    pip install dwave-neal

To build from source:

.. code-block:: bash

    pip install -r requirements.txt
    python setup.py build_ext --inplace
    python setup.py install

.. installation-end-marker

License
-------

Released under the Apache License 2.0. See LICENSE file.

Contribution
------------

See CONTRIBUTING.rst file.
