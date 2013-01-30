.. facebook/graph/fb_graph_notification.php generated using docpx on 01/30/13 03:58pm


Class
*****

FB_Graph_Notification
=====================

Methods
-------

setTemplate
+++++++++++

.. function:: setTemplate()


    Set template
    
    The template text to be shown to the user.


    :param string: 

    :rtype: void 



setHref
+++++++

.. function:: setHref()


    Set href
    
    The unique tracking data you want added to the url for tracking


    :param string: 

    :rtype: void 



getPost
+++++++

.. function:: getPost()


    Get post


    :rtype: array 



__construct
+++++++++++

.. function:: __construct()


    Constructor
    
    User mentions in the template should use the new syntax @[USER_ID]
    instead of the old syntax {USER_ID}


    :param string: the template text
    :param string: the tracking data added to the url

    :rtype: void 



create
++++++

.. function:: create()


    Create


    :param string|int: the user ID

    :rtype: boolean true if the post succeeded





Constants
---------

CONNECTION
++++++++++

