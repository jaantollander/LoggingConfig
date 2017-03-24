Python Tools for Setting up Logging
-----------------------------------

.. image:: https://badges.gitter.im/loggingtools/Lobby.svg
   :alt: Join the chat at https://gitter.im/loggingtools/Lobby
   :target: https://gitter.im/loggingtools/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
.. todo:: Command line client instruction

``setup_logging``

.. code-block:: python

   import logging
   from loggingtools import setup_logging
   setup_logging('logging.yaml')
   logger = logging.getLogger('<your_logger>')
   ...


``log_with``

.. code-block:: python

   import logging
   from loggingtools import setup_logging

   ...  # setup your loggers

   logger = logging.getLogger('<your_logger>')

   @log_with(logger)
   def function(arg, arg2):
       ...


Installation
------------
.. todo:: PyPI package

Currently can be installed through git

.. code-block:: bash

   pip install git+https://github.com/jaantollander/loggingtools.git


References
----------
https://docs.python.org/3/library/logging.html
https://github.com/borntyping/python-colorlog
