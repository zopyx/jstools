Release procedure
-----------------

Run the tests and make sure they all pass::

    $ python setup.py test

Edit the pavement.py file, set the ``version`` variable as appropriate, and
then commit and push the change.

Create a Git tag and push it to GitHub::

    $ git tag -a x.y -m 'version x.y'
    $ git push upstream tag x.y

``upstream`` is the name of the git@github.com:camptocamp/jstools.git remote
here.

Build a source package and upload it to pypi.python.org::

    $ python setup.py sdist upload
