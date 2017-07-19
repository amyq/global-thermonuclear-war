.. include:: _includes/acquia-products.txt

Basic text styles
*****************************************************


############################################################
This is a subheading.
############################################################

Links
=========
* single ``*asterisks*`` should get you *italics*
* double ``**asterisks**`` should get you **bolding**
* `python <www.python.org>`_ is a standard link
** but if you encase that same code in two backticks on each side, like this: ```python <www.python.org>`_`` you should get a literal

Lists
=========

* Asterisks for
* unordered lists

1. Use numbers for
2. Ordered lists
  a. Amy isn't thrilled about this requirement, FYI
  b. Craig will tell her to get over it


Directive boxes
======================

.. seealso:: This is a moderately simple **seealso** note.

.. note::  This is a **note** box.

.. tip::  Don't eat yellow snow.

.. warning:: note the space between the directive and the text

.. todo:: We also need to talk about anchors in the text.

About sections
======================

* If under and overline are used, their length must be identical.
* The length of the underline must be at least as long as the title itself

This is a sub-section
------------------------

A text block that is indented relative to the preceding text, without preceding markup indicating it to be a literal block or other content, is a block quote. All markup processing (for body elements and inline markup) continues within the block quote:

  Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?

This is a sub-sub-section
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When writing up sections, there are some conventions.

* ``#`` with overline, for parts
* ``*`` with overline, for chapters
* ``=``, for sections
* ``-``, for subsections
* ``^``, for subsubsections
* ``"``, for paragraphs

.. todo:: We need to discuss whether titles should have over- and under-lines. There are advantages and disadvantages.


Code-related
======================

Inline code is best done by wrapping your code ``in two backticks`` on each side

.. code-block:: php
    :linenos:

    <?php echo 'hello world!'; ?>
