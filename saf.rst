.. saf.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF
===

Methods
-------

__construct
+++++++++++

.. function:: __construct()


    Constructor


    :rtype: void 



instance
++++++++

.. function:: instance()


    Get instance


    :rtype: SAF 



__clone
+++++++

.. function:: __clone()


    Disallow cloning



createAlbum
+++++++++++

.. function:: createAlbum()


    Returns a Facebook Album


    :param string: 

    :rtype: FB_Graph_Album 



createCheckin
+++++++++++++

.. function:: createCheckin()


    Returns a Facebook Checkin


    :param string: the Place Page ID
    :param string: 
    :param string: 

    :rtype: FB_Graph_Checkin 



createComment
+++++++++++++

.. function:: createComment()


    Returns a Facebook Comment


    :param string: 

    :rtype: FB_Graph_Comment 



createEvent
+++++++++++

.. function:: createEvent()


    Returns a Facebook Event


    :param string: the event name
    :param string: the event start time, in ISO-8601

    :rtype: FB_Graph_Event 



createLink
++++++++++

.. function:: createLink()


    Returns a Facebook Link


    :param string: 

    :rtype: FB_Graph_Link 



createNote
++++++++++

.. function:: createNote()


    Returns a Facebook Note


    :param string: the subject
    :param string: the comment

    :rtype: FB_Graph_Note 



createNotification
++++++++++++++++++

.. function:: createNotification()


    Returns a Facebook Notification


    :param string: the template text
    :param string: the tracking data added to the url

    :rtype: FB_Graph_Notification 



createPost
++++++++++

.. function:: createPost()


    Returns a Facebook Post


    :param string: 

    :rtype: FB_Graph_Post 



createQuestion
++++++++++++++

.. function:: createQuestion()


    Returns a Facebook Question


    :param string: the text of the question

    :rtype: FB_Graph_Question 



