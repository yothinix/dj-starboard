=====
Usage
=====

To use starboard in a project, add it to your `INSTALLED_APPS`:

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
