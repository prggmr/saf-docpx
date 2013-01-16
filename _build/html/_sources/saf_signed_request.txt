.. /saf_signed_request.php generated using docpx on 01/16/13 09:23pm


SAF_Signed_Request
******************



Methods
=======

getUserId
---------

.. function:: getUserId()



getPageId
---------

.. function:: getPageId()



getAppData
----------

.. function:: getAppData()



isPageAdmin
-----------

.. function:: isPageAdmin()



isPageLiked
-----------

.. function:: isPageLiked()



isPageLikeViaFanGate
--------------------

.. function:: isPageLikeViaFanGate()



setExtendedAccessToken
----------------------

.. function:: setExtendedAccessToken()


    EXCHANGE SHORT-LIVED ACCESS TOKEN FOR A LONG-LIVED ACCESS TOKEN
    
    Overrides the Facebook SDK's setExtendedAccessToken() method.
    The Facebook SDK (3.2.2) doesn't set the access token property to the
    long-lived token for some strange reason so getAccessToken() will still
    return the short-lived token. So we have to get it from the app session
    where the Facebook SDK stores it and manually set the access token to the
    long-lived one.


    :rtype: void 



__construct
-----------

.. function:: __construct()


    CONSTRUCTOR


    :rtype: void 



_facebookConnect
----------------

.. function:: _facebookConnect()


    Facebook Connect
    
    Upon user login (authentication) Facebook Connect apps will have 'state'
    and 'code' parameters passed.  The code must be exchanged for an access
    token.


    :rtype: void 



_forceFacebookChrome
--------------------

.. function:: _forceFacebookChrome()


    FORCE FACEBOOK CHROME
    
    Ensure the user is viewing the tab or canvas app within the
    Facebook chrome.


    :rtype: string 



