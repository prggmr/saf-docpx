.. saf_session.php generated using docpx on 01/30/13 03:57pm


Class
*****

SAF_Session
===========

Methods
-------

getAppId
++++++++

.. function:: getAppId()



getPageData
+++++++++++

.. function:: getPageData()



getPageAccessToken
++++++++++++++++++

.. function:: getPageAccessToken()



getPageId
+++++++++

.. function:: getPageId()



getPageName
+++++++++++

.. function:: getPageName()



getPageProfileUrl
+++++++++++++++++

.. function:: getPageProfileUrl()



getPageProfilePicture
+++++++++++++++++++++

.. function:: getPageProfilePicture()



getPageLikes
++++++++++++

.. function:: getPageLikes()



getPageWebsite
++++++++++++++

.. function:: getPageWebsite()



getPageTabUrl
+++++++++++++

.. function:: getPageTabUrl()



getAddPageTabUrl
++++++++++++++++

.. function:: getAddPageTabUrl()



getCanvasUrl
++++++++++++

.. function:: getCanvasUrl()



isPageLiked
+++++++++++

.. function:: isPageLiked()



isPagePublished
+++++++++++++++

.. function:: isPagePublished()



hasPageRestrictions
+++++++++++++++++++

.. function:: hasPageRestrictions()



getUserData
+++++++++++

.. function:: getUserData()



getUserId
+++++++++

.. function:: getUserId()



getUserName
+++++++++++

.. function:: getUserName()



getUserFirstName
++++++++++++++++

.. function:: getUserFirstName()



getUserLastName
+++++++++++++++

.. function:: getUserLastName()



getUserGender
+++++++++++++

.. function:: getUserGender()



getUserEmail
++++++++++++

.. function:: getUserEmail()



getUserProfileUrl
+++++++++++++++++

.. function:: getUserProfileUrl()



getUserProfilePicture
+++++++++++++++++++++

.. function:: getUserProfilePicture()



getUserGrantedPerms
+++++++++++++++++++

.. function:: getUserGrantedPerms()



getUserRevokedPerms
+++++++++++++++++++

.. function:: getUserRevokedPerms()



isPageAdmin
+++++++++++

.. function:: isPageAdmin()



isAppDeveloper
++++++++++++++

.. function:: isAppDeveloper()



isAuthenticated
+++++++++++++++

.. function:: isAuthenticated()



hasPermission
+++++++++++++

.. function:: hasPermission()



__construct
+++++++++++

.. function:: __construct()


    CONSTRUCTOR


    :param string: app id for the SAF session we want to access

    :rtype: void 



setPersistentData
+++++++++++++++++

.. function:: setPersistentData()


    Stores the given ($key, $value) pair, so that future calls to
    getPersistentData($key) return $value. This call may be in another request.


    :param string: 
    :param mixed: 

    :rtype: void 



getPersistentData
+++++++++++++++++

.. function:: getPersistentData()


    Get the data for $key


    :param string: The key of the data to retrieve
    :param boolean: The default value to return if $key is not found

    :rtype: mixed 



_getPersistentSignedRequestData
+++++++++++++++++++++++++++++++

.. function:: _getPersistentSignedRequestData()


    Helper to get to signed request data sub key
    Actually returns $_SESSION['fb_APPID_saf_signed_request'][$key]


    :param string: The key of the data to retrieve
    :param boolean: The default value to return if $key is not found

    :rtype: mixed 



_getPersistentPageData
++++++++++++++++++++++

.. function:: _getPersistentPageData()


    Helper to get to page data sub key
    Actually returns $_SESSION['fb_APPID_saf_page][$key]


    :param string: The key of the data to retrieve
    :param boolean: The default value to return if $key is not found

    :rtype: mixed 



_getPersistentUserData
++++++++++++++++++++++

.. function:: _getPersistentUserData()


    Helper to get to user data sub key
    Actually returns $_SESSION['fb_APPID_saf_user][$key]


    :param string: The key of the data to retrieve
    :param boolean: The default value to return if $key is not found

    :rtype: mixed 



_constructSessionVariableName
+++++++++++++++++++++++++++++

.. function:: _constructSessionVariableName()


    Construct variable name just for our SAF persistent data
    eg - 'key' becomes 'fb_APPID_saf_key'
    
    access     private

    :rtype: void 



