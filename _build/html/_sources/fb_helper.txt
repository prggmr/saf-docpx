.. /fb_helper.php generated using docpx on 01/16/13 09:23pm


FB_Helper
*********



Methods
=======

meta
----

.. function:: meta()


    Returns a facebook open graph meta tag


    :param string: property of tag
    :param string: content of tag

    :rtype: string 



picture_url
-----------

.. function:: picture_url()


    Returns the Facebook picture url


    :param int: 
    :param string: square (50x50), small (50x?), normal (100x?) or large (200x?)

    :rtype: string 



profile_url
-----------

.. function:: profile_url()


    Returns the Facebook profile url


    :param int: 

    :rtype: string 



fan_page_url
------------

.. function:: fan_page_url()


    Returns the Facebook fan page url


    :param int: 

    :rtype: string 



page_tab_url
------------

.. function:: page_tab_url()


    Returns the Facebook fan page tab url


    :param int: (eg - pages/X-Studios/262672746449)
    :param int: 

    :rtype: string 



add_page_tab_url
----------------

.. function:: add_page_tab_url()


    Returns the url needed to add the app as a page tab


    :param int: 
    :param string: 

    :rtype: string 



login_link
----------

.. function:: login_link()


    Returns the link needed to correctly login a user
    Works for both a tab or canvas app


    :param string: 

    :rtype: string 



logout_link
-----------

.. function:: logout_link()


    Returns the link needed to correctly logout a user
    Works for both a tab or canvas app


    :param string: 

    :rtype: string 



graph_request
-------------

.. function:: graph_request()


    Returns public info from the Facebook graph api
    Most of the time Facebook will respond with JSON data,
    but there are special cases where it will not


    :param int: id of the object we want public info for
    :param bool: decode json response

    :rtype: mixed 



