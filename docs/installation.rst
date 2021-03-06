Installation
============

Compatibility
-------------
* Python: 2.6, 2.7
* Django: 1.4, 1.5, 1.6, 1.7, 1.8


Installation
------------
Recommended way to install is via pip:

.. code-block:: bash

    $ pip install django-db-mailer

    # do not forget collect your project static on production servers
    $ python manage.py collectstatic


.. _basic:

Settings configuration
----------------------

Add ``dbmail`` to ``INSTALLED_APPS`` in the settings.py:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'dbmail',
        ...
    )


DB initialization
-----------------

Create application tables on database:

.. code-block:: bash

    $ python manage.py syncdb


If you're using South:


.. code-block:: bash

    $ python manage.py migrate


**Important:** South 1.0 or greater is required to run this migrations.
