.. saf_page_connection.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF_Page_Connection
===================

Methods
-------

__construct
+++++++++++

.. function:: __construct()


    Constructor


    :param SAF_Page: 
    :param SAF: 

    :rtype: void 



getConnection
+++++++++++++

.. function:: getConnection()


    Get a page connection


    :param string: connection name
    :param array: query params

    :rtype: mixed 



getAdmins
+++++++++

.. function:: getAdmins()


    Returns a list of the page's admins.


    :rtype: array of objects containing id, name



getAlbums
+++++++++

.. function:: getAlbums()


    Returns the photo albums the page has uploaded.


    :rtype: array of album objects



getBlocked
++++++++++

.. function:: getBlocked()


    Returns a list of users blocked from the page.


    :rtype: array of objects containing id, name



getCheckins
+++++++++++

.. function:: getCheckins()


    Returns the checkins made to this place page by the
    current user, and friends of the current user.
    
    Permissions: user_checkins or friends_checkins


    :rtype: array of checkin objects



getConversations
++++++++++++++++

.. function:: getConversations()


    Returns a list of the page's conversations.
    
    Permissions: Page access token with read_mailbox permission


    :rtype: array of checkin objects



getEvents
+++++++++

.. function:: getEvents()


    Returns the events the page is attending.


    :rtype: array of event objects



getFeed
+++++++

.. function:: getFeed()


    Get the page's wall.


    :rtype: array of Post objects



getGlobalBrandChildren
++++++++++++++++++++++

.. function:: getGlobalBrandChildren()


    Returns information of all children pages.


    :rtype: array of JSON objects



getGroups
+++++++++

.. function:: getGroups()


    Returns the groups to which the page belongs.


    :rtype: array array containing group id, version, name & unread fields



getInsights
+++++++++++

.. function:: getInsights()


    Get the page's Insights data.
    
    Permissions: read_insights permission


    :rtype: array of insights objects



getLinks
++++++++

.. function:: getLinks()


    Returns the the page's posted links.


    :rtype: array of link objects



getMilestones
+++++++++++++

.. function:: getMilestones()


    Returns a list of the page's milestones.


    :rtype: array of milestone objects



getNotes
++++++++

.. function:: getNotes()


    Returns the page's notes.


    :rtype: array of note objects



getPhotos
+++++++++

.. function:: getPhotos()


    Returns the page's uploaded photos.


    :rtype: array of Photo objects



getPicture
++++++++++

.. function:: getPicture()


    Returns the page's profile picture.


    :param string: square, small, normal, large

    :rtype: string URL of the page's profile picture



getPosts
++++++++

.. function:: getPosts()


    Returns the page's own posts.


    :rtype: array of post objects



getPromotablePosts
++++++++++++++++++

.. function:: getPromotablePosts()


    Returns the page's own posts, including unpublished
    and scheduled posts.


    :rtype: array of post objects



getQuestions
++++++++++++

.. function:: getQuestions()


    Returns the page's questions.


    :rtype: array of question objects



getSettings
+++++++++++

.. function:: getSettings()


    Returns the page's settings.


    :rtype: array of objects containing setting and value fields



getStatuses
+++++++++++

.. function:: getStatuses()


    Returns the page's status updates.


    :rtype: array of status message objects



getTabs
+++++++

.. function:: getTabs()


    Returns the page's tabs.
    
    Permissions: Page access token


    :rtype: array of tab objects



getTagged
+++++++++

.. function:: getTagged()


    Returns the photos, videos, and posts in which the Page has been tagged.


    :rtype: array of Photo, Video or Post objects



getVideos
+++++++++

.. function:: getVideos()


    Returns the videos the page has uploaded.


    :rtype: array of video objects



_getPageAccessToken
+++++++++++++++++++

.. function:: _getPageAccessToken()


    Get the page's access token.



    :rtype: string 



