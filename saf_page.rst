.. saf_page.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF_Page
========

Methods
-------

getId
+++++

.. function:: getId()


    Returns the page ID


    :rtype: string|int 



getData
+++++++

.. function:: getData()


    Returns the page data


    :rtype: array 



getAccessToken
++++++++++++++

.. function:: getAccessToken()


    Returns the page's access token


    :rtype: string 



getName
+++++++

.. function:: getName()


    Returns the page's name


    :rtype: string 



getProfileUrl
+++++++++++++

.. function:: getProfileUrl()


    Returns the page's profile URL


    :rtype: string 



getProfilePicture
+++++++++++++++++

.. function:: getProfilePicture()


    Returns the page's profile picture


    :rtype: string 



getLikes
++++++++

.. function:: getLikes()


    Returns the page's like count


    :rtype: string|int 



getWebsite
++++++++++

.. function:: getWebsite()


    Returns the page's website


    :rtype: string 



getTabUrl
+++++++++

.. function:: getTabUrl()


    Returns the app tab URL


    :rtype: string 



getAddTabUrl
++++++++++++

.. function:: getAddTabUrl()


    Returns the URL needed to add the app to a page


    :rtype: string 



isPublished
+++++++++++

.. function:: isPublished()


    Returns true if the page is published


    :rtype: boolean 



isLiked
+++++++

.. function:: isLiked()


    Returns true if the user likes this page


    :rtype: boolean 



hasRestrictions
+++++++++++++++

.. function:: hasRestrictions()


    Returns true if the page has restrictions


    :rtype: boolean 



getRssUrl
+++++++++

.. function:: getRssUrl()


    Returns the page's RSS URL


    :rtype: string 



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



_injectSAFData
++++++++++++++

.. function:: _injectSAFData()


    Add our own useful social app framework parameter(s) to the page data


    :rtype: array 



_getValue
+++++++++

.. function:: _getValue()


    Returns a page key value whether it exists or not


    :param string: key to check for
    :param mixed: default value if not set

    :rtype: mixed 





Constants
---------

RSS
+++

