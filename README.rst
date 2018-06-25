=============================
starboard
=============================

.. image:: https://badge.fury.io/py/dj-starboard.svg
    :target: https://badge.fury.io/py/dj-starboard

.. image:: https://travis-ci.org/yothinix/dj-starboard.svg?branch=master
    :target: https://travis-ci.org/yothinix/dj-starboard

.. image:: https://codecov.io/gh/yothinix/dj-starboard/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/yothinix/dj-starboard

Django Starboard is a providing mechanism that allow data synchronization between Django  project as easy as possible. Suitable for building fleet of microservices based on Django.

Documentation
-------------

The full documentation is at https://dj-starboard.readthedocs.io.

Quickstart
----------

Install starboard::

    pip install dj-starboard

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'starboard.apps.StarboardConfig',
        ...
    )

Add starboard's URL patterns:

.. code-block:: python

    from starboard import urls as starboard_urls


    urlpatterns = [
        ...
        url(r'^', include(starboard_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
