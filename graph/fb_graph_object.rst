.. facebook/graph/fb_graph_object.php generated using docpx on 01/30/13 03:58pm


Class
*****

FB_Graph_Object
===============

Methods
-------

__construct
+++++++++++

.. function:: __construct()


    Constructor


    :rtype: void 



delete
++++++

.. function:: delete()


    Delete an object
    
    Note that some objects can't be deleted: checkins, albums, notifications


    :param string|int: the object ID

    :rtype: boolean true if the delete succeeded



_verifyPermission
+++++++++++++++++

.. function:: _verifyPermission()


    Verify permissions


    :rtype: void 



