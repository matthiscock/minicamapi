API - Authorisation
===================

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
