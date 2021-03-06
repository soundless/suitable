Suitable
========

An Ansible API for humans.

Documentation
-------------

`<http://suitable.readthedocs.org>`_

Warning
-------

Suitable is not endorsed by Ansible and it is not affilated with it. Use at
your own peril.

The official way to use Ansible from Python is documented here:
`<http://docs.ansible.com/ansible/developing_api.html>`_

Run Tests
---------

.. code-block:: python

    pip install tox
    tox

Build Status
------------

.. image:: https://travis-ci.org/seantis/suitable.svg?branch=master
    :target: https://travis-ci.org/seantis/suitable
    :alt: Build status

Test Coverage
-------------

.. image:: https://codecov.io/github/seantis/suitable/coverage.svg?branch=master
    :target: https://codecov.io/github/seantis/suitable?branch=master
    :alt: Test coverage

Latest Release
--------------

.. image:: https://badge.fury.io/py/suitable.svg
    :target: https://badge.fury.io/py/suitable
    :alt: Latest release

Changelog
---------
0.7.4 (2017-01-27)
~~~~~~~~~~~~~~~~~~~

- Fixes an issue with Ansible 2.1.4.0. Host lists are now passed to Ansible in
  a format it expects.
  [href]

0.7.3 (2016-03-08)
~~~~~~~~~~~~~~~~~~~

- Gets password based ssh authentication working again.
  [href]

0.7.2 (2016-01-15)
~~~~~~~~~~~~~~~~~~~

- Stops command and shell modules from chocking on certain commands.
  Workaround for https://github.com/ansible/ansible/issues/13862
  [href]

0.7.1 (2016-01-15)
~~~~~~~~~~~~~~~~~~~

- Removes global state lingering around with Ansible 2.0.0.2, which introduced
  a hosts cache leading to Suitable's api instances to not be independent.
  [href]

0.7.0 (2016-01-13)
~~~~~~~~~~~~~~~~~~~

- Adds support for Ansible 2.0. **Does not support 1.x anymore!!**
  [href]

0.6 (2015-06-22)
~~~~~~~~~~~~~~~~

- Adds backwards-compatible support for Ansible 1.9. The same code running on
  suitable for Ansible 1.8 should now work with Ansible 1.9.
  [href]

0.5 (2014-11-28)
~~~~~~~~~~~~~~~~

- Adds support for Ansible 1.8.
  [href]

- Includes automated tests for Ansible versions 1.5 through 1.8.
  [href]

- Properly escapes spaces in key-value pairs. Fixes #3.
  [href]

0.4 (2014-09-05)
~~~~~~~~~~~~~~~~

- Wraps the result of all module runs to provide easy access to results
  per server.
  [href]

- Default to transport 'localhost' if 'localhost' or '127.0.0.1' is used
  exclusively on the API object.
  [href]

0.3 (2014-05-28)
~~~~~~~~~~~~~~~~

- Adds a stern warning so users won't confuse this with the official Ansible API.
  [href]

0.2 (2014-05-21)
~~~~~~~~~~~~~~~~

- Change license to GPL v3 as required by Ansible.
  [href]

0.1 (2014-05-21)
~~~~~~~~~~~~~~~~

- Initial release.
  [href]
