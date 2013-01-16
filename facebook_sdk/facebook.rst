.. /facebook_sdk/facebook.php generated using docpx on 01/16/13 09:23pm


Facebook
********


Extends the BaseFacebook class with the intent of using
PHP sessions to store user ids and access tokens.



Methods
=======

__construct
-----------

.. function:: __construct()


    Identical to the parent constructor, except that
    we start a PHP session to store the user ID and
    access token if during the course of execution
    we discover them.

    :param Array: the application configuration. Additionally
accepts "sharedSession" as a boolean to turn on a secondary
cookie for environments with a shared session (that is, your app
shares the domain with other apps).

    :see : 



initSharedSession
-----------------

.. function:: initSharedSession()



setPersistentData
-----------------

.. function:: setPersistentData()


    Provides the implementations of the inherited abstract
    methods.  The implementation uses PHP sessions to maintain
    a store for authorization codes, user ids, CSRF states, and
    access tokens.



getPersistentData
-----------------

.. function:: getPersistentData()



clearPersistentData
-------------------

.. function:: clearPersistentData()



clearAllPersistentData
----------------------

.. function:: clearAllPersistentData()



deleteSharedSessionCookie
-------------------------

.. function:: deleteSharedSessionCookie()



getSharedSessionCookieName
--------------------------

.. function:: getSharedSessionCookieName()



constructSessionVariableName
----------------------------

.. function:: constructSessionVariableName()





Constants
---------

FBSS_COOKIE_NAME
++++++++++++++++

FBSS_COOKIE_EXPIRE
++++++++++++++++++

