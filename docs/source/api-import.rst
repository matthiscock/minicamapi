API - Imports
===

Import XMLs
------------

Purpose
~~~~~~~

The purpose of this end point is for the Solo Pro to get one or more XML files, which match the setup and formatting which the current import uses, and import these as Wincan Projects.

If the project exists it will append any new sections found. (but not overwrite any).


Requests and Params
~~~~~~~~~~~~~~~~~~~

.. code-block:: php

   Endpoint: /api/v1/minican/getProjects
   
   Header:
      Authorization : 'bearer ' + token
   
   Post:
      Null
      
   Returns: 
      Json { response, xmlFiles } 


Desired Actions
~~~~~~~~~~~~~~~

* Import from Footprint button
* Select a user
* Footprint returns XML (as string, as files, as zip, whichever is easier)
* They are imported using the existing import mechanism within the solo pro - all sections imported
* (existing sections are not over written)


