Release procedure
-----------------

Run the tests and make sure they all pass::

    (env) $ python setup.py test

Edit the pavement.py file, set the ``version`` variable as appropriate, and
then commit and push the change.

Build a source package::

    (env) $ python setup.py sdist

Upload to pypi.python.org::

    (env) $ python setup.py upload
