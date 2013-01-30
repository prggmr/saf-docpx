.. facebook/graph/fb_graph_question.php generated using docpx on 01/30/13 03:58pm


Class
*****

FB_Graph_Question
=================

Methods
-------

setQuestion
+++++++++++

.. function:: setQuestion()


    Set question
    
    The text of the question


    :param string: 

    :rtype: void 



setOptions
++++++++++

.. function:: setOptions()


    Set options
    
    Array of answer options


    :param array: 

    :rtype: void 



setAllowNewOptions
++++++++++++++++++

.. function:: setAllowNewOptions()


    Set allow new options
    
    Allows other users to add new options (True by default)


    :param boolean: 

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
    
    Requires extended permission: publish_stream


    :param string: the text of the question

    :rtype: void 



create
++++++

.. function:: create()


    Create a question


    :param string|int: the profile ID (eg - me)

    :rtype: string the new question ID





Constants
---------

CONNECTION
++++++++++

