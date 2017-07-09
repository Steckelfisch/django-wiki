Developer guide
===============

.. toctree::
   :maxdepth: 1

   environment
   testproject
   testing

.. highlight:: shell


Types of Contributions
----------------------

Report Bugs
~~~~~~~~~~~

Report bugs at https://github.com/django-wiki/django-wiki/issues.

If you are reporting a bug, please include:

* Your operating system name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* Detailed steps to reproduce the bug.

Fix Bugs
~~~~~~~~

Look through the GitHub issues for bugs. Anything tagged with "bug"
and "help wanted" is open to whoever wants to implement it.

Implement Features
~~~~~~~~~~~~~~~~~~

Look through the GitHub issues for features. Anything tagged with "enhancement"
and "help wanted" is open to whoever wants to implement it.

Write Documentation
~~~~~~~~~~~~~~~~~~~

Django-wiki could always use more documentation, whether as part of the
official django-wiki docs, in docstrings, or even on the web in blog posts,
articles, and such.

Submit Feedback
~~~~~~~~~~~~~~~

The best way to send feedback is to file an issue at https://github.com/django-wiki/django-wiki/issues.

If you are proposing a feature:

* Explain in detail how it would work.
* Keep the scope as narrow as possible, to make it easier to implement.
* Remember that this is a volunteer-driven project, and that contributions
  are welcome :)

Get Started!
------------

Ready to contribute? Here's how to set up `django-wiki` for local development.

1. Fork the `django-wiki` repo on GitHub.
2. Clone your fork locally::

    $ git clone git@github.com:your_name_here/django-wiki.git

3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::

    $ mkvirtualenv django-wiki
    $ cd django-wiki/
    $ python setup.py develop

4. Create a branch for local development::

    $ git checkout -b name-of-your-bugfix-or-feature

   Now you can make your changes locally.

5. When you're done making changes, check that your changes pass flake8 and the tests, including testing other Python versions with tox::

    $ tox -e lint
    $ py.test  # Run tests in current environment
    $ tox

   To get flake8 and tox, just pip install them into your virtualenv.

6. Commit your changes and push your branch to GitHub::

    $ git add .
    $ git commit -m "Your detailed description of your changes."
    $ git push origin name-of-your-bugfix-or-feature

7. Submit a pull request through the GitHub website.

Pull Request Guidelines
-----------------------

Before you submit a pull request, check that it meets these guidelines:

1. The pull request should include tests.
2. If the pull request adds functionality, the docs should be updated. Put
   your new functionality into a function with a docstring, and add the
   feature to the list in README.rst.
3. The pull request should work for Python 2.6, 2.7, 3.3, 3.4 and 3.5, and for PyPy. Check
   https://travis-ci.org/django-wiki/django-wiki/pull_requests
   and make sure that the tests pass for all supported Python versions.

Tips
----

To run a subset of tests::

    $ py.test tests.test_django-wiki


Roadmap
-------

The best way to contribute is to use our Github issue list to look
at current wishes. The list is found here:

https://github.com/django-wiki/django-wiki/issues/

If you want to add a feature, consider writing a plugin. Please create an
issue to discuss whether your plugin idea is a core plugin
(``wiki.plugins.*``) or external plugin. If there are additions needed
to the plugin API, we can discuss that as well! A discussion is always welcome
in a Github issue.

Generally speaking, we need more **unit tests** to improve coverage, and new
features will not be accepted without tests. To add more stuff to the project
without tests wouldn't be fair to the project or your hard work. We use coverage
metrics to see that each new contribution does not significantly impact test
coverage.
