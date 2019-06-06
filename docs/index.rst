readthedocs-sphinx-search
=========================

This version uses the ``sphinx-es-suggest`` extension: https://github.com/rtfd/readthedocs-sphinx-search

Once built, search suggestions should show when user starts typing in the search bar.

* When the page finished loading, there should be additional <div> nodes
  in the DOM (above the <body> tag).
* Search modal should open (with the backdrop) when user clicks on the search input field
  when was already present.
* Search modal should close if the user clicks on "cross icon" at the top-right corner
  of the modal, user presses "Escape" button or user clicks on the backdrop.
* User should be able to iterate through the results by ArrowUp/ArrowDown buttons.
  There should be smooth scrolling.
* When the search modal appears, there should be no previous results or previous query.

.. toctree::
   :glob:
   :caption: Table of Contents

   *


----

Sphinx configuration file to build this docs (:doc:`see full file <conf>`),

.. literalinclude:: conf.py
   :language: python
   :end-before: ###########################################################################
   :linenos:

----

.. runblock:: pycon

   >>> # Build at
   >>> import datetime
   >>> datetime.datetime.utcnow()  # UTC
