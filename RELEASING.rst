Release procedure
-----------------

Run the tests and make sure they all pass::

    $ python setup.py test

Edit the pavement.py file, set the ``version`` variable as appropriate, and
then commit and push the change.

Create a Git tag and push it to GitHub::

    $ git tag -a x.y -m 'version x.y'
    $ git push tag x.y

Build a source package::

    $ python setup.py sdist

Upload to pypi.python.org::

    $ python setup.py upload
