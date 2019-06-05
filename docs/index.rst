sphinx-es-suggest
=================

This version uses the ``sphinx-es-suggest`` extension: https://github.com/rtfd/sphinx-es-suggest

Once built, search suggestions should show when user starts typing in the search bar.

* DOM elements are created and destroyed dynamically.
  This can be checked via the Chrome Inspect Tool.
* User can loop through the results via "ArrowUp" and "ArrowDown" keys.
* If "Enter" key is pressed and an suggestion is selected (either from ArrowUp or ArrowDown),
  user is taken to the correspoding result link.
  If no suggestion is selected, search form is submitted.
* If suggestions are open, and the user clicks somewhere else on the page,
  except the input field, results are removed.
* If suggestions are open, and the user presses "Escape" button,
  results are removed.
* In case there is an error while fetching the results,
  show error to the user.
* In case, no results are found, notify the user.

.. toctree::
    :maxdepth: 2
    :caption: Table of Contents

    about-rtd
    frameworks


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
