=============================
Python2.7 for Debian Squeeze
=============================

My python2.7 buildout for `Plone`_ on `Debian Squeeze`_

.. contents:: :local:

**Disclaimer**: you should use the official supported `collective buildout.python`_ or the `Unified Installer`_


This buildout works for me, but it is just a dirty and quick workaround.

Dependencies
------------

Install at least readline, zlib and build-essential, usually I install more, till I want to setup `Plone`_ anyway::

    apt-get install wget build-essential wv poppler-utils python2.6-dev python-imaging libssl-dev libjpeg62-dev zlib1g-dev libreadline5-dev libxml2-dev python-libxml2 libxslt1


Install
-------

Usually I install it into $USER/opt::

    mkdir $USER/opt

Further::

    cd opt
    git clone https://github.com/svx/squeeze-python27.git
    cd squeeze-python
    python bootstrap.py
    ./bin/buildout


.. _Plone: https://plone.org/
.. _Debian Squeeze: http://www.debian.org/releases/stable/
.. _collective buildout.python: https://github.com/collective/buildout.python
.. _Unified Installer: https://plone.org/documentation/manual/installing-plone/installing-on-linux-unix-bsd/what-is-the-unified-installer


