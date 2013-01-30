.. saf_facebook.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF_Facebook
============

Methods
-------

__construct
+++++++++++

.. function:: __construct()


    Constructor


    :rtype: void 



_init
+++++

.. function:: _init()


    Init


    :rtype: void 



getAppAccessToken
+++++++++++++++++

.. function:: getAppAccessToken()


    Returns the app's access token


    :rtype: string|int 



getLoginUrl
+++++++++++

.. function:: getLoginUrl()


    Returns the login URL
    
    Override's the Facebook SDK's native method


    :param array: parameters to pass

    :rtype: string 



getLogoutUrl
++++++++++++

.. function:: getLogoutUrl()


    Returns the logout URL
    
    Override's the Facebook SDK's native method


    :param array: parameters to pass

    :rtype: string 



getLoginLink
++++++++++++

.. function:: getLoginLink()


    Returns the login link (anchor tag)


    :rtype: string 



getLogoutLink
+++++++++++++

.. function:: getLogoutLink()


    Returns the logout link (anchor tag)


    :rtype: string 



getExtendedPerms
++++++++++++++++

.. function:: getExtendedPerms()


    Returns the permissions the app requested


    :rtype: string comma delimited string of perms



setExtendedPerms
++++++++++++++++

.. function:: setExtendedPerms()


    Sets the extended perms to be used with getLoginURL();


    :param string: delimited perms

    :rtype: void 



getRedirectUrl
++++++++++++++

.. function:: getRedirectUrl()


    Returns the redirect URL to be used with getLoginUrl()


    :rtype: string 



setRedirectUrl
++++++++++++++

.. function:: setRedirectUrl()


    Sets the redirect URL to be used with getLoginUrl()


    :param string: 

    :rtype: void 



setExtendedAccessToken
++++++++++++++++++++++

.. function:: setExtendedAccessToken()


    Overrides the Facebook SDK's setExtendedAccessToken() method.
    The Facebook SDK (3.2.2) doesn't set the access token property to the
    long-lived token for some strange reason so getAccessToken() will still
    return the short-lived token. So we have to get it from the app session
    where the Facebook SDK stores it and manually set the access token to the
    long-lived one.


    :rtype: void 



_determineRedirectUrl
+++++++++++++++++++++

.. function:: _determineRedirectUrl()


    Returns the proper redirect URL for use with getLoginUrl()


    :rtype: string 



debug
+++++

.. function:: debug()


    Wrapper around an external class so we can do a simple check if the
    class (XS_Debug) is avaliable before we attempt to use its method.


    :param string: name, label, message
    :param var: a variable
    :param int: (1)log, (2)info, (3)warn, (4)error
    :param bool: log to text file

    :rtype: void 





Constants
---------

SAF_VERSION
+++++++++++

