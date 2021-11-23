API
===

Import XMLs
------------

The purpose of this end point is for the Solo Pro to get one or more XML files, which match the setup and formatting which the current import uses, and import these as Wincan Projects.

If the project exists it will append any new sections found. (but not overwrite any).

.. code-block:: php

   Endpoint: /api/v1/minican/getWincanProjects
   
   



.. code-block:: console

   (.venv) $ pip install lumache

Send to Footprint
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:
