Template for the Read the Docs tutorial
=======================================

This GitHub template includes fictional Python library
with some basic Sphinx docs.

Read the tutorial here:

https://docs.readthedocs.io/en/stable/tutorial/

Getting Started
---------------

To start editing the group wiki, you'll need Python with **Sphinx** installed.
This can be done through ``pip``, and involves installing the packages
``sphinx`` and ``sphinx-rtd-theme``.
You will also need ``sphinx-copybutton`` as well.

Alternatively, you can get all the Python dependences in a virtual environment
by running the following commands in the repository's root folder ::

    python3 -m venv .venv
    source .venv/bin/activate
    pip install -r requirements.txt
    deactivate

This virtual environment can be used to build the website locally to view edits
you have made.
To activate it ``source`` the activation script in the ``/.venv/bin/``
directory, and to deactivate it run ``deactivate`` in the terminal.

The pages can be found in the ``/docs/source`` directory, with the homepage
labeled ``index.rst``.
The existing pages can be edited in place to update them, and a new page can be
created by creating a new ``.rst`` file alongside the others and adding the
filename to the ``.. toctree::`` table of contents in ``index.rst``.

To build the website pages, simply ``cd`` into the ``docs`` directory and run
``make html``.
If you also want to build a LaTeX pdf version of the docs, run
``make latexpdf``.
The built files can be viewed in ``/docs/build``.
To view the website, you can just open ``/docs/build/html/index.html`` in a
browser.
You can keep this *local version* of the website open and simply refresh the
page to see changes you make after re-building.
