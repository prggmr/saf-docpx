.. facebook/graph/fb_graph_post.php generated using docpx on 01/30/13 03:58pm


Class
*****

FB_Graph_Post
=============

Methods
-------

setCaption
++++++++++

.. function:: setCaption()


    Set caption
    
    Post caption (can only be used if link is specified)


    :param string: 

    :rtype: void 



setDescription
++++++++++++++

.. function:: setDescription()


    Set description
    
    Post description (can only be used if link is specified)


    :param string: 

    :rtype: void 



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
    
    The message that appears in the post.


    :param string: 

    :rtype: void 



setName
+++++++

.. function:: setName()


    Set name
    
    Post name (can only be used if link is specified)


    :param string: 

    :rtype: void 



setPicture
++++++++++

.. function:: setPicture()


    Set picture
    
    Post thumbnail image (can only be used if link is specified)


    :param string: 

    :rtype: void 



setActions
++++++++++

.. function:: setActions()


    Set actions
    
    Array of objects containing 'name' and 'link' keys


    :param array: 

    :rtype: void 



setTargeting
++++++++++++

.. function:: setTargeting()


    Set targeting
    
    JSON object containing countries, cities, regions or locales
    Example: {'countries':['US','GB']}


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


    :param string: the message

    :rtype: void 



createAction
++++++++++++

.. function:: createAction()


    Create action
    
    Returns an associative array for an action link


    :param $name: name
    :param $link: value

    :rtype: array 



createProperty
++++++++++++++

.. function:: createProperty()


    Create property
    
    Returns an associative array for a property link


    :param $text: text
    :param $href: 

    :rtype: array 



create
++++++

.. function:: create()


    Create a post


    :param string|int: the profile ID (eg - me)

    :rtype: string the new post ID





Constants
---------

CONNECTION
++++++++++

