.. saf_user.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF_User
========

Methods
-------

getId
+++++

.. function:: getId()


    Returns user's Facebook ID


    :rtype: string|int 



getData
+++++++

.. function:: getData()


    Returns the user data


    :rtype: array 



getFirstName
++++++++++++

.. function:: getFirstName()


    Returns the user's first name


    :rtype: string 



getLastName
+++++++++++

.. function:: getLastName()


    Returns the user's last name


    :rtype: string 



getName
+++++++

.. function:: getName()


    Returns the user's full name


    :rtype: string 



getGender
+++++++++

.. function:: getGender()


    Returns the user's gender


    :rtype: string 



getEmail
++++++++

.. function:: getEmail()


    Returns the user's email


    :rtype: string 



getAgeRange
+++++++++++

.. function:: getAgeRange()


    Returns the user's age range


    :rtype: object containing min and max



getProfileUrl
+++++++++++++

.. function:: getProfileUrl()


    Returns the user's profile URL


    :rtype: string 



getProfilePicture
+++++++++++++++++

.. function:: getProfilePicture()


    Returns the user's profile picture URL


    :rtype: string 



getGrantedPerms
+++++++++++++++

.. function:: getGrantedPerms()


    Returns the permissions the user granted


    :rtype: array 



getRevokedPerms
+++++++++++++++

.. function:: getRevokedPerms()


    Returns the permissions the user revoked


    :rtype: array 



isAppDeveloper
++++++++++++++

.. function:: isAppDeveloper()


    Returns true if the user is the app developer


    :rtype: string 



isAuthenticated
+++++++++++++++

.. function:: isAuthenticated()


    Returns true if the user is authenticated


    :rtype: boolean 



hasPermission
+++++++++++++

.. function:: hasPermission()


    Returns true if a user has permission


    :param string: permission to check

    :rtype: boolean 



__construct
+++++++++++

.. function:: __construct()


    Constructor


    :param SAF_Facebook: 
    :param string|int: 

    :rtype: void 



_init
+++++

.. function:: _init()


    Init


    :rtype: void 



_thirdPartyCookieFix
++++++++++++++++++++

.. function:: _thirdPartyCookieFix()


    Checks if a session cookie is not set and if so, automatically redirects
    the user to the base URL with a 'saf_redirect' URL param. The app then
    starts the session on the 'real' server and immediately redirects back
    to the proper URL (tab or convas);


    :rtype: string 



_isAppDeveloper
+++++++++++++++

.. function:: _isAppDeveloper()


    Returns true if the user is the app developer


    :rtype: boolean 



_checkPermissions
+++++++++++++++++

.. function:: _checkPermissions()


    Check permissions


    :rtype: void 



_getValue
+++++++++

.. function:: _getValue()


    Returns a user key value whether it exists or not


    :param string: key to check for
    :param mixed: default value if not set

    :rtype: mixed 



