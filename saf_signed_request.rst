.. saf_signed_request.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF_Signed_Request
==================

Methods
-------

getUserId
+++++++++

.. function:: getUserId()


    Returns the user ID


    :rtype: string|int 



getPageId
+++++++++

.. function:: getPageId()


    Returns the page ID


    :rtype: string|int 



getAppData
++++++++++

.. function:: getAppData()


    Returns the app data


    :rtype: mixed 



isPageAdmin
+++++++++++

.. function:: isPageAdmin()


    Returns true if the user is the page admin


    :rtype: boolean 



isPageLiked
+++++++++++

.. function:: isPageLiked()


    Returns true if the user likes this page


    :rtype: boolean 



isPageLikeViaFanGate
++++++++++++++++++++

.. function:: isPageLikeViaFanGate()


    Returns true if the page was liked via fan gate


    :rtype: boolean 



__construct
+++++++++++

.. function:: __construct()


    Constructor


    :param SAF_Base: 

    :rtype: void 



_init
+++++

.. function:: _init()


    Init


    :rtype: void 



_forceFacebookChrome
++++++++++++++++++++

.. function:: _forceFacebookChrome()


    Ensure the user is viewing the tab or canvas app within the
    Facebook chrome.


    :rtype: string 



