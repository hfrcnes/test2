Makefile
========

This chapter aims to list all the makefile targets and explain what they do :

- ``build`` : it starts the command ``poetry build``, which builds the lib into the dist folder.
- ``build_docs`` : it builds the docs using Sphinx commands, to mirror the current state of sources
- ``format`` : it uses the python tool black_ to format the source code to make it cleaner, this command is meant to be used occasionally to cleanup the whole code 
- ``lint_source`` : it uses the python tool flake8_ to lint the source code
- ``lint_tests`` : same for the tests code
- ``serve_docs`` : it serves the html docs on your hpc cluster using the proxy and gives you the link to access it
- ``full_docs`` : it's a simple combination of ``build_docs`` and ``serve_docs``
- ``test`` : it runs all the tests contained in the ``tests`` folder
- ``test_utils`` : it runs all the tests contained in the ``tests/utils`` folder, as the test ``test_geodes`` can be long, it can be useful to not include in some tests sessions
- ``publish`` : to publish to Artifactory

.. _black: https://black.readthedocs.io/en/stable/
.. _flake8: https://flake8.pycqa.org/en/latest/
