API - Exports
=============


Send Project to Footprint
----------------

Purpose
~~~~~~~

The purpose of this end point is to allow a project and all files to be sent to Footprint.
This is generally the same as Wincan Web

You may wish to have several end points - one for the project and then seperate endpoint for each file - all of which is fine. Ive assumed this is the case


Requests and Params
~~~~~~~~~~~~~~~~~~~

.. code-block:: php

   Endpoint: /api/v1/minican/recieveProject
   
   Header:
      Authorization : 'bearer ' + token
   
   Post:
      Files (as a zip or whatever pleases yourselves)
      
   Returns: 
      Json { response } (success or fail)


Desired Actions
~~~~~~~~~~~~~~~

The project is sent to Footprint.  A confirmation message is shown to the user when complete.
      

------------
      

Send File to Footprint
----------------

Purpose
~~~~~~~

Send a file to Footprint


Requests and Params
~~~~~~~~~~~~~~~~~~~

.. code-block:: php

   Endpoint: /api/v1/minican/recieveProject
   
   Header:
      Authorization : 'bearer ' + token
   
   Post:
      Files (as a zip or whatever pleases yourselves)
      
   Returns: 
      Json { response } (success or fail)


Desired Actions
~~~~~~~~~~~~~~~

The project is sent to Footprint.  A confirmation message is shown to the user when complete.
   


