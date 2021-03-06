********
profiles
********

Summary: Create and manage application users

create: Create new user profile
===============================
``profiles.create(body=<BODY>)``

Keyword Args:
-------------
    * **body**: The profile information for a new user (JSON, string)


Response:
---------
    * *A single Profile object*

list: List user profiles
========================
``profiles.list(email=None, first_name=None, full_name=None, last_name=None, limit=250, name=None, offset=0, status=None, username=None)``

Keyword Args:
-------------
    * **email**: Filter results by email. (string, optional)
    * **first_name**: Filter results by first_name. (string, optional)
    * **full_name**: Filter results by full_name. (string, optional)
    * **last_name**: Filter results by last_name. (string, optional)
    * **limit**: The max number of results. (integer, optional)
    * **name**: Filter results by name. (string, optional)
    * **offset**: The number of records to when returning the results. When paginating results, the page number = ceil(offset/limit) (integer, optional)
    * **status**: Filter results by status. (string, optional)
    * **username**: Filter results by username. (string, optional)


Response:
---------
    * *Array of Profile objects*

get: Find authenticated user profile
====================================
``profiles.get()``

Response:
---------
    * *A single Profile object*

delete: Delete user profile
===========================
``profiles.delete(username=<USERNAME>)``

Keyword Args:
-------------
    * **username**: The username of a valid api user (string)


Response:
---------
    * *A single Profile object*

listByUsername: Find api user profile by their api username
===========================================================
``profiles.listByUsername(username=<USERNAME>)``

Keyword Args:
-------------
    * **username**: The username of a valid api user (string)


Response:
---------
    * *A single Profile object*

update: Update user profile
===========================
``profiles.update(body=<BODY>, username=<USERNAME>)``

Keyword Args:
-------------
    * **body**: Updated profile information for a user (JSON, string)
    * **username**: The username of a valid api user (string)


Response:
---------
    * *A single Profile object*

