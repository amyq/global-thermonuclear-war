..  _styles-advanced:
Advanced text styles
*****************************************************

If |ACSF| looks like "Acquia Cloud Site Factory" then the quick-and-dirty substitution file works.

Long-term, I think we want to take this approach instead, placing this chunk in ``conf.py``, source https://docs.chef.io/style_guide.html#rst-prolog

.. code-block:: python

  # A string of reStructuredText that will be included at the beginning of every source file that is read.
  rst_prolog = """
  .. include:: ../../swaps/swap_descriptions.txt
  .. include:: ../../swaps/swap_names.txt
  """

Text substitutions
=====================
``rst.prolog`` is defined in ``conf.py`` per http://widequestion.com/question/automatically-include-definitions-file-from-subdirectories/  and points to two text files in the ``_includes`` folder. (The different file name extension is to avoid Sphinx finding it as a standalone document.)

http://docutils.sourceforge.net/docs/ref/rst/directives.html#include

See http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html#substitution-definitions



Images
======================

.. image:: images/cats.jpg

Figures
=============

Figures are images with captions

.. figure:: images/cats.jpg
  :scale: 50 %

  Beryl and Kolohe.

.. todo:: Should image paths begin with a slash or without one? We should figure that out.

Topics
======================
.. topic:: Your Topic Title

    Subsequent indented lines comprise
    the body of the topic, and are
    interpreted as body elements.

Tables
======================
.. csv-table:: a title
   :header: "name", "firstname", "age"
   :widths: 20, 20, 10

   "Smith", "John", 40
   "Smith", "John, Junior", 20


.. todo:: Glossaries?

.. todo:: Nested lists that contain ordered and unordered items

Definition lists
======================

item
  definition here

second item
  definition here


Option lists
===============
Somewhere out there, I saw a version that had some gorgeous styling, but I can't find what I had.
http://louistiao.me/posts/demos/restructuredtext-demo/#option-lists has some decent style

From reading https://gist.github.com/ionelmc/e876b73e2001acd2140f it looks like it's using the ``<kbd>`` tag.

-a            command-line option "a"
-b file       options can have arguments
              and long descriptions
--long        options can be long also
--input=file  long options can also have
              arguments
/V            DOS/VMS-style options too


Blockquoting
===============
A paragraph containing only two colons indicates
the following indented or quoted text is a literal
block or quoted text is a literal block.

::

  Whitespace, newlines, blank lines, and  all kinds of
  markup (like *this* or \this) is preserved here.

Per-line quoting can also be used for unindented
blocks:

> Useful for quotes from email and


Theming
========
Our theme is Bootstrap, from http://sphinx-bootstrap-theme.readthedocs.io/ (there's another Bootstrap theme but it's for mkdocs, not Sphinx.)

.. todo:: Investigate ToC tree for sidebar (default is h2s on page are imported to sidebar) https://stackoverflow.com/questions/18969093/how-to-include-the-toctree-in-the-sidebar-of-each-page
