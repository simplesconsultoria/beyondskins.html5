=================
beyondskins.html5
=================

Introduction
============

*Beyondskins HTML5* Theme is an installable Plone Theme developed by 
`Simples Consultoria`_ using the **theming** and **packaging** 
features available in `plone.app.theming`_.

Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*will be installed as a dependency of this package*)


Screenshots
===========

Layout of the site when viewed in a computer resolution:

.. image:: https://github.com/simplesconsultoria/beyondskins.html5/raw/master/beyondskins/html5/static/preview.png


Features
========

- It's an installable Plone Theme package.
- After installation from Add-ons controlpanel, this theme is enabled automatically.
- Also it's a simple Diazo package (Zip file).
- It's have support for clean uninstallation.


Installation
============


Zip file
--------

If you are an end user, you might enjoy installation via zip file import.

1. Download a `zip file <https://github.com/simplesconsultoria/beyondskins.html5/raw/master/beyondskins.html5.zip>`_.
2. Import the theme from the Diazo theme control panel.

Enabling the theme
^^^^^^^^^^^^^^^^^^

Select and enable the theme from the Diazo control panel. That's it!


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``beyondskins.html5`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        beyondskins.html5


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'beyondskins.html5',
    ],


Usage
=====

The *Beyondskins HTML5* theme for Plone is a Diazo Theme based on HTML5 
for Simples Consultoria Website

This is a very basic and clean Plone theme that uses HTML5 tags in your 
structure and gives you a Semantic HTML to start your projects.


HTML
----

Instead a lot of `div>`tags, this theme uses new HTML5 tags like 
`header> section> <nav> and <footer>`


Styles
------


CSS Reset
^^^^^^^^^

Beyondskins HTML5 use `Normalize.css`_ to reset the styles. ``Normalize.css`` 
makes browsers render all elements more consistently and in line with modern 
standards. It precisely targets only the styles that need normalizing.


Grid
^^^^

Beyondskins HTML5 doesn't use any grid system, mainly because the actual grid 
systems make a mess in your html, adding a lot of non semantical tags. And 
because you don't need a grid system to create a website with 2 or 3 columns.

To change columns size, just edit grid.css file included ins this package: ::

    #main {width: 100%;}
    #main-content {width: auto;}
    #column-one {width: 16%;}
    #column-two {width: 30%;}

If you need a grid system, just plug your favorite grid system following their 
instructions. With a little mess in the HTML file you can make any modern grid 
system to work here.


Responsive
----------

Yes


Scripts
-------

To do



Contribute
==========

- Issue Tracker: https://github.com/simplesconsultoria/beyondskins.html5/issues
- Source Code: https://github.com/simplesconsultoria/beyondskins.html5


License
=======

The project is licensed under the GPLv2.

Credits
-------

- Andre Nogueira (agnogueira at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/agnogueira/beyondskins.html5/contributors

.. _`Simples Consultoria`: http://www.simplesconsultoria.com.br/
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`Normalize.css`: http://necolas.github.io/normalize.css/
