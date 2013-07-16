============
Installation
============

For Contributors
----------------

These instructions assume that you want to do active development on both
django-admin2 and djadmin2-theme-naturale.

Create a virtualenv::

    virtualenv djadmin2-env

Install your fork of django-admin2 for local development, using the 
djadmin2-theme-naturale branch::

    git clone git@github.com:your-name-here/django-admin2.git
    cd django-admin2
    git checkout -b djadmin2-theme-naturale
    python setup.py develop

Install your fork of djadmin2-theme-naturale for local development::

    git clone git@github.com:your-name-here/djadmin2-theme-naturale.git
    cd djadmin2-theme-naturale
    python setup.py develop

Add this to the settings.py of the django-admin2 example project::

    INSTALLED_APPS = (
        # ... snip the rest
        'djadmin2',
        'djadmin2_naturale'
    )

    ########## ADMIN2 CONFIGURATION
    ADMIN2_THEME_DIRECTORY = "djadmin2_naturale"
    ########## END ADMIN2 CONFIGURATION

For End Users
-------------

This package is still in active development. It's not ready for regular use yet.
