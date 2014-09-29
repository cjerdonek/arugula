Releasing Arugula
=================

TODO: copy information from groome-python-expected.


### Register the release on PyPI

Once the repository is ready, register the version on PyPI.

Registering on PyPI adds an entry to PyPI for the version without uploading
any code.  Registering creates a page and URL for the version
(e.g. [http://pypi.python.org/pypi/Pizza/0.1.0](http://pypi.python.org/pypi/Pizza/0.1.0)),
stores metadata about the version, and adds the current "long_description"
to the version's page after converting it to HTML.

The [Python Packaging User Guide][pug] recommends using the
[registration form][pypi-registration] on the PyPI web site since this
method is secure.  Using `python setup.py register` is insecure because
it passes your credentials in plain-text.

Each time you create a new version for release, you should register that
version.  If you make a mistake or find that the metadata is not correct
after registering, it is okay to correct the source code and register again.
Subsequent registrations will overwrite the metadata previously stored for
that version.


[pug]: https://packaging.python.org/en/latest/index.html
[pypi-registration]: https://pypi.python.org/pypi?%3Aaction=submit_form
