.. facebook/graph/fb_graph_link.php generated using docpx on 01/30/13 03:58pm


Class
*****

FB_Graph_Link
=============

Methods
-------

setLink
+++++++

.. function:: setLink()


    Set link
    
    The link attached to this post


    :param string: 

    :rtype: void 



setMessage
++++++++++

.. function:: setMessage()


    Set message


    :param string: 

    :rtype: void 



setPublished
++++++++++++

.. function:: setPublished()


    Set published
    
    Whether a post is published. Default is published.
    
    Requires extended permissions: publish_stream, manage_pages
    Only available when publishing to a page.


    :param boolean: 

    :rtype: void 



setScheduledPublishTime
+++++++++++++++++++++++

.. function:: setScheduledPublishTime()


    Set scheduled publish time
    
    Time when the page post should go live, this should be between 10 mins
    and 6 months from the time of publishing the post.
    
    Requires extended permissions: publish_stream, manage_pages
    Only available when publishing to a page.


    :param string: a unix timestamp

    :rtype: void 



__construct
+++++++++++

.. function:: __construct()


    Constructor


    :param string: the url

    :rtype: void 



create
++++++

.. function:: create()


    Create a link


    :param string|int: the profile ID (eg - me)

    :rtype: string the new link ID





Constants
---------

CONNECTION
++++++++++

