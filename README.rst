
Rapidsmsapp
========================

Below you will find basic setup instructions for the ``rapidsmsapp``
project. To begin you should have the following applications installed on your
local development system:

- `Python >= 2.7 (including Python 3) <http://www.python.org/getit/>`_
- `pip >= 7.0.3 <http://www.pip-installer.org/>`_
- `virtualenv >= 13.0.3 <http://www.virtualenv.org/>`_

Getting Started
---------------

To setup your local environment you should create a virtualenv and install the
necessary requirements::

    virtualenv rapidsmsapp-env

On Posix systems you can activate your environment like this::

    source rapidsmsapp-env/bin/activate

On Windows, you'd use::

    rapidsmsapp-env\Scripts\activate

Then::

    cd rapidsmsapp
    pip install -U -r requirements/base.txt

Run migrate::

    python manage.py migrate

You should now be able to run the development server::

    python manage.py runserver
