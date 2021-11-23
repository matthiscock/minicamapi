API
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



Send to Footprint
----------------
Purpose
~~~~~~~

The purpose of this end point is to allow a project and all files to be sent to Footprint.
This is generally the same as Wincan Web


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
      
      
      
      
   





Authorise A User
----------------

Purpose
~~~~~~~

The purpose of this end point is to allow a user to get and send information to Footprint.
A token (which lasts forever) is given to allow this to happen without the need to authorise everytime.
Tokens are managed in Footprint for ease


Requests and Params
~~~~~~~~~~~~~~~~~~~

.. code-block:: php

   Endpoint: /api/v1/minican/authoriseUser
   
   Post:
      username, password
      
   Returns: 
      Json { response, name, lastname, token }


Desired Actions
~~~~~~~~~~~~~~~

This user is stored on the system.





De - Authorise A User
----------------

Purpose
~~~~~~~

The purpose of this end point is to allow a user to be removed from the system.  It does not need to contact Footprint.


Desired Actions
~~~~~~~~~~~~~~~

* List of users which are authorised shown
* Choose a User
* This user is removed from the system.
