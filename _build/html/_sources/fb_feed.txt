.. /fb_feed.php generated using docpx on 01/16/13 09:23pm


FB_Feed
*******



Methods
=======

setFacebook
-----------

.. function:: setFacebook()


    SET FACEBOOK
    
    Set the facebook sdk instance


    :param $facebook: SDK instance

    :rtype: void 



setAccessToken
--------------

.. function:: setAccessToken()


    SET ACCESS TOKEN
    
    Set the access token to use


    :param $token: token

    :rtype: void 



setFrom
-------

.. function:: setFrom()


    SET FROM
    
    The ID or username of the user posting the message.
    If this is unspecified, it defaults to the current user.
    If specified, it must be the ID of the user or of a
    page that the user administers


    :param $user_id: 

    :rtype: void 



setTo
-----

.. function:: setTo()


    SET TO
    
    The ID or username of the profile that this story will be
    published to. If this is unspecified, it defaults to the
    value of from.


    :param $user_id: 

    :rtype: void 



setLink
-------

.. function:: setLink()


    SET LINK
    
    The link attached to this post


    :param $url: 

    :rtype: void 



setPicture
----------

.. function:: setPicture()


    SET PICTURE
    
    The URL of a picture attached to this post. The picture
    must be at least 50px by 50px and have a maximum aspect
    ratio of 3:1


    :param $url: 

    :rtype: void 



setSource
---------

.. function:: setSource()


    SET SOURCE
    
    The URL of a media file (either SWF or MP3) attached to
    this post. If both source and picture are specified,
    only source is used.


    :param $url: 

    :rtype: void 



setName
-------

.. function:: setName()


    SET NAME
    
    The name of the link attachment.


    :param $value: 

    :rtype: void 



setCaption
----------

.. function:: setCaption()


    SET CAPTION
    
    The caption of the link (appears beneath the link name).
    If not specified, this field is automatically populated
    with the URL of the link.


    :param $value: 

    :rtype: void 



setDescription
--------------

.. function:: setDescription()


    SET DESCRIPTION
    
    The description of the link (appears beneath the link
    caption). If not specified, this field is automatically
    populated by information scraped from the link,
    typically the title of the page.


    :param $value: 

    :rtype: void 



setMessage
----------

.. function:: setMessage()


    SET MESSAGE
    
    The message that appears in the post. Facebook
    suggests not pre-populating this parameter?


    :param $value: 

    :rtype: void 



setProperties
-------------

.. function:: setProperties()


    SET PROPERTIES
    
    A JSON object of key/value pairs which will appear in
    the stream attachment beneath the description, with
    each property on its own line. Keys must be strings,
    and values can be either strings or JSON objects with
    the keys text and href.


    :param $json_obj: 

    :rtype: void 



setActions
----------

.. function:: setActions()


    SET ACTIONS
    
    A JSON array containing a single object describing the
    action link which will appear next to the "Comment"
    and "Like" link under posts. The contained object must
    have the keys name and link.


    :param $json_obj: 

    :rtype: void 



setRef
------

.. function:: setRef()


    SET REF
    
    A text reference for the category of feed post. This
    category is used in Facebook Insights to help you
    measure the performance of different types of post


    :param $json_obj: 

    :rtype: void 



__construct
-----------

.. function:: __construct()


    CONSTRUCTOR


    :param $facebook: SDK instance (can be set later before publish is called)

    :rtype: void 



publish
-------

.. function:: publish()


    PUBLISH
    
    Publish a facebook feed and returns an object
    with success or failure info


    :param $profile_id: of the user/page to publish to
    :param $type: or page eg - FB_PublishFeed::TYPE_USER

    :rtype: object 



createAction
------------

.. function:: createAction()


    CREATE ACTION
    
    Returns an associative array for an action link


    :param $name: name
    :param $link: value

    :rtype: array 



createProperty
--------------

.. function:: createProperty()


    CREATE PROPERTY
    
    Returns an associative array for an property link


    :param $name: 
    :param $text: text
    :param $href: 

    :rtype: array 



_publishData
------------

.. function:: _publishData()


    PUBLISH DATA
    
    Returns an associative array with only valid (non null) params


    :rtype: array 





Constants
---------

TYPE_USER
+++++++++

TYPE_PAGE
+++++++++

