.. start-badges

| |gh_actions| |codecov|
| |pypi| |supported-versions| |supported-implementations|

.. |gh_actions| image:: https://img.shields.io/github/actions/workflow/status/Rockhopper-Technologies/ansicon/tests.yml?event=push&logo=github-actions&style=plastic
    :target: https://github.com/Rockhopper-Technologies/ansicon/actions/workflows/tests.yml
    :alt: GitHub Actions Status

.. |appveyor| image:: https://img.shields.io/appveyor/ci/Rockhopper-Technologies/ansicon.svg?style=plastic&logo=appveyor
    :target: https://ci.appveyor.com/project/Rockhopper-Technologies/ansicon
    :alt: Appveyor Build Status

.. |coveralls| image:: https://img.shields.io/coveralls/github/Rockhopper-Technologies/ansicon.svg?style=plastic&logo=coveralls
    :target: https://coveralls.io/github/Rockhopper-Technologies/ansicon
    :alt: Coverage Status

.. |codecov| image:: https://img.shields.io/codecov/c/github/Rockhopper-Technologies/ansicon.svg?style=plastic&logo=codecov
    :target: https://codecov.io/gh/Rockhopper-Technologies/ansicon
    :alt: Coverage Status

.. |pypi| image:: https://img.shields.io/pypi/v/ansicon.svg?style=plastic&logo=pypi
    :alt: PyPI Package latest release
    :target: https://pypi.python.org/pypi/ansicon

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/ansicon.svg?style=plastic&logo=pypi
    :alt: Supported versions
    :target: https://pypi.python.org/pypi/ansicon

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/ansicon.svg?style=plastic&logo=pypi
    :alt: Supported implementations
    :target: https://pypi.python.org/pypi/ansicon

.. end-badges

Overview
========
ansicon is a Python wrapper for loading `Jason Hood`_'s ANSICON_


Installation
============

.. code-block:: console

    $ pip install ansicon


Usage
=====

.. code-block:: python

    import ansicon

    # Load ansicon
    ansicon.load()

    # Have fun with terminal codes
    print(u'\x1b[32mGreen\x1b[m')

    # Unload ansicon
    ansicon.unload()

    # Check if ansicon is loaded
    if not ansicon.loaded():
        ansicon.load()
    if ansicon.loaded():
        ansicon.unload()

.. _Jason Hood: https://github.com/adoxa
.. _ANSICON: https://github.com/adoxa/ansicon