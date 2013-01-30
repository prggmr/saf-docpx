.. saf_user_connection.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF_User_Connection
===================

Methods
-------

__construct
+++++++++++

.. function:: __construct()


    Constructor


    :param SAF_User: 
    :param SAF: 

    :rtype: void 



getConnection
+++++++++++++

.. function:: getConnection()


    Get a user connection


    :param string: connection name
    :param array: query params

    :rtype: mixed 



getAccounts
+++++++++++

.. function:: getAccounts()


    Returns the pages owned by the current user.
    
    Permissions: manage_pages


    :rtype: array of objects



getAchievements
+++++++++++++++

.. function:: getAchievements()


    Returns the achievements for the user.
    
    Permissions: user_games_activity or friends_games_activity


    :rtype: array of objects



getActivities
+++++++++++++

.. function:: getActivities()


    Returns the activities listed on the user's profile.
    
    Permissions: user_activities or friends_activities


    :rtype: array of objects



getAlbums
+++++++++

.. function:: getAlbums()


    Returns the photo albums the user has created.
    
    Permissions: user_photos or friends_photos


    :rtype: array of album objects



getApplications
+++++++++++++++

.. function:: getApplications()


    Returns the apps owned by the current user.
    
    Permissions: manage_pages


    :rtype: array of objects



getAppRequests
++++++++++++++

.. function:: getAppRequests()


    Returns the user's outstanding requests from an app.
    
    Permissions: app access token


    :rtype: array of app requests



getBooks
++++++++

.. function:: getBooks()


    Returns the books listed on the user's profile.
    
    Permissions: user_likes or friends_likes


    :rtype: array of objects



getCheckins
+++++++++++

.. function:: getCheckins()


    Returns the places that the user has checked-into.
    
    Permissions: user_checkins or friends_checkins


    :rtype: array of checkin objects



getEvents
+++++++++

.. function:: getEvents()


    Returns the events this user is attending.
    
    Permissions: user_events or friends_events


    :rtype: array of objects



getFamily
+++++++++

.. function:: getFamily()


    Returns the user's family relationships.
    
    Permissions: user_relationships


    :rtype: array of objects



getFeed
+++++++

.. function:: getFeed()


    Returns the users's wall.
    
    Permissions: read_stream


    :rtype: array of post objects



getFriends
++++++++++

.. function:: getFriends()


    Returns the user's friends.


    :rtype: array of objects



getFriendLists
++++++++++++++

.. function:: getFriendLists()


    Returns the user's friend lists.
    
    Permissions: read_friendlists


    :rtype: array of post objects



getFriendRequests
+++++++++++++++++

.. function:: getFriendRequests()


    Returns the user's incoming friend requests.
    
    Permissions: read_requests


    :rtype: array of objects



getGames
++++++++

.. function:: getGames()


    Returns the games the user has added to the Arts and
    Entertainment section of their profile.
    
    Permissions: user_likes


    :rtype: array of objects



getGroups
+++++++++

.. function:: getGroups()


    Returns the groups that the user belongs to.
    
    Permissions: user_groups or friends_groups


    :rtype: array of objects



getNewsFeed
+++++++++++

.. function:: getNewsFeed()


    Returns the user's news feed.
    
    Permissions: read_stream


    :rtype: array of post objects



getInbox
++++++++

.. function:: getInbox()


    Returns the threads in this user's inbox.
    
    Permissions: read_mailbox


    :rtype: array of thread objects



getInterests
++++++++++++

.. function:: getInterests()


    Returns the interests listed on the user's profile.
    
    Permissions: user_interests or friends_interests


    :rtype: array of objects



getLikes
++++++++

.. function:: getLikes()


    Returns the pages this user has liked.
    
    Permissions: user_likes or friends_likes


    :rtype: array of objects



getLinks
++++++++

.. function:: getLinks()


    Returns the user's posted links.
    
    Permissions: read_stream


    :rtype: array of link objects



getLocations
++++++++++++

.. function:: getLocations()


    Returns the posts, statuses, and photos in which the user has
    been tagged at a location, or where the user has authored
    content.
    
    Permissions: user_photos, friend_photos, user_status,
    friends_status, user_checkins, or friends_checkins.


    :rtype: array of objects



getMovies
+++++++++

.. function:: getMovies()


    Returns the movies listed on the user's profile.
    
    Permissions: user_likes or friends_likes.


    :rtype: array of objects



getMusic
++++++++

.. function:: getMusic()


    Returns the music listed on the user's profile.
    
    Permissions: user_likes or friends_likes


    :rtype: array of objects



getMutualFriends
++++++++++++++++

.. function:: getMutualFriends()


    Returns the mutual friends between two users.


    :rtype: array of objects



getNotes
++++++++

.. function:: getNotes()


    Returns the user's notes.
    
    Permissions: read_stream


    :rtype: array of objects



getNotifications
++++++++++++++++

.. function:: getNotifications()


    Returns the app notifications for the user.
    
    Permissions: manage_notifications


    :rtype: array of objects



getOutbox
+++++++++

.. function:: getOutbox()


    Returns the messages in this user's outbox.
    
    Permissions: read_mailbox


    :rtype: array of objects



getPayments
+++++++++++

.. function:: getPayments()


    Returns the Facebook Credits orders the user placed with
    an application. Requires application to be payments enabled.
    
    Permissions: app access token


    :rtype: array of objects



getPermissions
++++++++++++++

.. function:: getPermissions()


    Returns the permissions that user has granted the application.


    :rtype: array a single object with keys as the permission name



getPhotos
+++++++++

.. function:: getPhotos()


    Returns the photos the user (or friend) is tagged in.


    :rtype: array of photo objects



getPhotosUploaded
+++++++++++++++++

.. function:: getPhotosUploaded()


    Returns the photos of a user.
    
    Permissions: user_photos


    :rtype: array of photo objects



getPicture
++++++++++

.. function:: getPicture()


    Get the user's profile picture.


    :param string: square, small, normal, large

    :rtype: string URL of the user'sprofile picture



getPokes
++++++++

.. function:: getPokes()


    Returns the user's pokes.
    
    Permissions: read_mailbox


    :rtype: array of objects



getPosts
++++++++

.. function:: getPosts()


    Returns the user's own posts.
    
    Permissions: read_stream for non-public posts


    :param boolean: return non-public posts as well

    :rtype: array of post objects



getQuestions
++++++++++++

.. function:: getQuestions()


    Returns the user's questions.
    
    Permissions: user_questions


    :rtype: array of question objects



getScores
+++++++++

.. function:: getScores()


    Returns the current scores for the user in games.
    
    Permissions: user_games_activity or friends_games_activity


    :rtype: array of objects



getSharedPosts
++++++++++++++

.. function:: getSharedPosts()


    Returns the shares of the object.
    
    Permissions: read_stream


    :rtype: array of post objects



getStatuses
+++++++++++

.. function:: getStatuses()


    Returns the user's status updates.
    
    Permissions: read_stream


    :rtype: array of post objects



getSubscribedTo
+++++++++++++++

.. function:: getSubscribedTo()


    Returns the people the user is subscribed to.


    :rtype: array of objects



getSubscribers
++++++++++++++

.. function:: getSubscribers()


    Returns the user's subscribers.


    :rtype: array of objects



getTagged
+++++++++

.. function:: getTagged()


    Returns the posts the user is tagged in.
    
    Permissions: read_stream


    :rtype: array of objects



getTelevision
+++++++++++++

.. function:: getTelevision()


    Returns the television listed on the user's profile.
    
    Permissions: user_likes or friends_likes


    :rtype: array of objects



getUpdates
++++++++++

.. function:: getUpdates()


    Returns the updates in this user's inbox.
    
    Permissions: read_mailbox


    :rtype: array of objects



getVideos
+++++++++

.. function:: getVideos()


    Returns the videos this user has been tagged in.
    
    Permissions: user_videos or friends_videos


    :rtype: array of video objects



_checkPermission
++++++++++++++++

.. function:: _checkPermission()


    Check the user's permissions



    :rtype: void 



