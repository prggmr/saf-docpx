.. /saf_facebook_user.php generated using docpx on 01/16/13 09:23pm


SAF_Facebook_User
*****************



Methods
=======

getUserData
-----------

.. function:: getUserData()



getUserName
-----------

.. function:: getUserName()



getUserFirstName
----------------

.. function:: getUserFirstName()



getUserLastName
---------------

.. function:: getUserLastName()



getUserGender
-------------

.. function:: getUserGender()



getUserEmail
------------

.. function:: getUserEmail()



getUserProfileUrl
-----------------

.. function:: getUserProfileUrl()



getUserProfilePicture
---------------------

.. function:: getUserProfilePicture()



getExtendedPerms
----------------

.. function:: getExtendedPerms()



getGrantedPerms
---------------

.. function:: getGrantedPerms()



getRevokedPerms
---------------

.. function:: getRevokedPerms()



getLoginUrl
-----------

.. function:: getLoginUrl()



getLogoutUrl
------------

.. function:: getLogoutUrl()



getLoginLink
------------

.. function:: getLoginLink()



getLogoutLink
-------------

.. function:: getLogoutLink()



isAppDeveloper
--------------

.. function:: isAppDeveloper()



isAuthenticated
---------------

.. function:: isAuthenticated()



hasPermission
-------------

.. function:: hasPermission()


    CHECK IF USER HAS PERMISSION
    Determine if a user has allowed a specific permission


    :param string: permission to check

    :rtype: bool 



setRedirectUrl
--------------

.. function:: setRedirectUrl()



__construct
-----------

.. function:: __construct()


    CONSTRUCTOR


    :rtype: void 



_thirdPartyCookieFix
--------------------

.. function:: _thirdPartyCookieFix()


    THIRD PARTY COOKIE FIX
    
    Checks if a session cookie is not set and if so, automatically redirects
    the user to the base URL with a 'saf_redirect' URL param. The app then
    starts the session on the 'real' server and immediately redirects back
    to the proper URL (tab or convas);


    :rtype: string 



_determineRedirectUrl
---------------------

.. function:: _determineRedirectUrl()


    DETERMINE REDIRECT URL
    
    Returns the proper redirect URL for use with getLoginUrl()


    :rtype: string 



_handleException
----------------

.. function:: _handleException()


    HANDLE EXCEPTION


    :rtype: void 



_isAppDeveloper
---------------

.. function:: _isAppDeveloper()


    DETERMINE IF USER IS THE APP DEVELOPER


    :rtype: boolean 



_checkPermissions
-----------------

.. function:: _checkPermissions()


    CHECK PERMISSIONS


    :rtype: void 



_getUserValue
-------------

.. function:: _getUserValue()


    GET USER VALUE
    
    Return a clean value whether the key exits or not


    :param string: key to check for
    :param mixed: default value if not set

    :rtype: mixed 



