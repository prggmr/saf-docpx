.. /facebook_sdk/base_facebook.php generated using docpx on 01/16/13 09:23pm


FacebookApiException
********************


Thrown when an API call returns an exception.



Methods
=======

__construct
-----------

.. function:: __construct()


    Make a new API Exception with the given result.

    :param array: The result from the API server



getResult
---------

.. function:: getResult()


    Return the associated result object returned by the API server.

    :rtype: array The result from the API server



getType
-------

.. function:: getType()


    Returns the associated type for the error. This will default to
    'Exception' when a type is not available.

    :rtype: string 



__toString
----------

.. function:: __toString()


    To make debugging easier.

    :rtype: string The string representation of the error



BaseFacebook
************


Provides access to the Facebook Platform.  This class provides
a majority of the functionality needed, but the class is abstract
because it is designed to be sub-classed.  The subclass must
implement the four abstract methods listed at the bottom of
the file.



Methods
=======

__construct
-----------

.. function:: __construct()


    Initialize a Facebook Application.
    
    The configuration:
    - appId: the application ID
    - secret: the application secret
    - fileUpload: (optional) boolean indicating if file uploads are enabled

    :param array: The application configuration



setAppId
--------

.. function:: setAppId()


    Set the Application ID.

    :param string: The Application ID

    :rtype: BaseFacebook 



getAppId
--------

.. function:: getAppId()


    Get the Application ID.

    :rtype: string the Application ID



setApiSecret
------------

.. function:: setApiSecret()


    Set the App Secret.

    :param string: The App Secret

    :rtype: BaseFacebook 

    :deprecated:  



setAppSecret
------------

.. function:: setAppSecret()


    Set the App Secret.

    :param string: The App Secret

    :rtype: BaseFacebook 



getApiSecret
------------

.. function:: getApiSecret()


    Get the App Secret.

    :rtype: string the App Secret

    :deprecated:  



getAppSecret
------------

.. function:: getAppSecret()


    Get the App Secret.

    :rtype: string the App Secret



setFileUploadSupport
--------------------

.. function:: setFileUploadSupport()


    Set the file upload support status.

    :param boolean: The file upload support status.

    :rtype: BaseFacebook 



getFileUploadSupport
--------------------

.. function:: getFileUploadSupport()


    Get the file upload support status.

    :rtype: boolean true if and only if the server supports file upload.



useFileUploadSupport
--------------------

.. function:: useFileUploadSupport()


    DEPRECATED! Please use getFileUploadSupport instead.
    
    Get the file upload support status.

    :rtype: boolean true if and only if the server supports file upload.



setAccessToken
--------------

.. function:: setAccessToken()


    Sets the access token for api calls.  Use this if you get
    your access token by other means and just want the SDK
    to use it.

    :param string: an access token.

    :rtype: BaseFacebook 



setExtendedAccessToken
----------------------

.. function:: setExtendedAccessToken()


    Extend an access token, while removing the short-lived token that might
    have been generated via client-side flow. Thanks to http://bit.ly/b0Pt0H
    for the workaround.



getAccessToken
--------------

.. function:: getAccessToken()


    Determines the access token that should be used for API calls.
    The first time this is called, $this->accessToken is set equal
    to either a valid user access token, or it's set to the application
    access token if a valid user access token wasn't available.  Subsequent
    calls return whatever the first call returned.

    :rtype: string The access token



getUserAccessToken
------------------

.. function:: getUserAccessToken()


    Determines and returns the user access token, first using
    the signed request if present, and then falling back on
    the authorization code if present.  The intent is to
    return a valid user access token, or false if one is determined
    to not be available.

    :rtype: string A valid user access token, or false if one
               could not be determined.



getSignedRequest
----------------

.. function:: getSignedRequest()


    Retrieve the signed request, either from a request parameter or,
    if not present, from a cookie.

    :rtype: string the signed request, if available, or null otherwise.



getUser
-------

.. function:: getUser()


    Get the UID of the connected user, or 0
    if the Facebook user is not connected.

    :rtype: string the UID if available.



getUserFromAvailableData
------------------------

.. function:: getUserFromAvailableData()


    Determines the connected user by first examining any signed
    requests, then considering an authorization code, and then
    falling back to any persistent store storing the user.

    :rtype: integer The id of the connected Facebook user,
                or 0 if no such user exists.



getLoginUrl
-----------

.. function:: getLoginUrl()


    Get a Login URL for use with redirects. By default, full page redirect is
    assumed. If you are using the generated URL with a window.open() call in
    JavaScript, you can pass in display=popup as part of the $params.
    
    The parameters:
    - redirect_uri: the url to go to after a successful login
    - scope: comma separated list of requested extended perms

    :param array: Provide custom parameters

    :rtype: string The URL for the login flow



getLogoutUrl
------------

.. function:: getLogoutUrl()


    Get a Logout URL suitable for use with redirects.
    
    The parameters:
    - next: the url to go to after a successful logout

    :param array: Provide custom parameters

    :rtype: string The URL for the logout flow



getLoginStatusUrl
-----------------

.. function:: getLoginStatusUrl()


    Get a login status URL to fetch the status from Facebook.
    
    The parameters:
    - ok_session: the URL to go to if a session is found
    - no_session: the URL to go to if the user is not connected
    - no_user: the URL to go to if the user is not signed into facebook

    :param array: Provide custom parameters

    :rtype: string The URL for the logout flow



api
---

.. function:: api()


    Make an API call.

    :rtype: mixed The decoded response



getSignedRequestCookieName
--------------------------

.. function:: getSignedRequestCookieName()


    Constructs and returns the name of the cookie that
    potentially houses the signed request for the app user.
    The cookie is not set by the BaseFacebook class, but
    it may be set by the JavaScript SDK.

    :rtype: string the name of the cookie that would house
        the signed request value.



getMetadataCookieName
---------------------

.. function:: getMetadataCookieName()


    Constructs and returns the name of the coookie that potentially contain
    metadata. The cookie is not set by the BaseFacebook class, but it may be
    set by the JavaScript SDK.

    :rtype: string the name of the cookie that would house metadata.



getCode
-------

.. function:: getCode()


    Get the authorization code from the query parameters, if it exists,
    and otherwise return false to signal no authorization code was
    discoverable.

    :rtype: mixed The authorization code, or false if the authorization
              code could not be determined.



getUserFromAccessToken
----------------------

.. function:: getUserFromAccessToken()


    Retrieves the UID with the understanding that
    $this->accessToken has already been set and is
    seemingly legitimate.  It relies on Facebook's Graph API
    to retrieve user information and then extract
    the user ID.

    :rtype: integer Returns the UID of the Facebook user, or 0
                if the Facebook user could not be determined.



getApplicationAccessToken
-------------------------

.. function:: getApplicationAccessToken()


    Returns the access token that should be used for logged out
    users when no authorization code is available.

    :rtype: string The application access token, useful for gathering
               public information about users and applications.



establishCSRFTokenState
-----------------------

.. function:: establishCSRFTokenState()


    Lays down a CSRF state token for this process.

    :rtype: void 



getAccessTokenFromCode
----------------------

.. function:: getAccessTokenFromCode()


    Retrieves an access token for the given authorization code
    (previously generated from www.facebook.com on behalf of
    a specific user).  The authorization code is sent to graph.facebook.com
    and a legitimate access token is generated provided the access token
    and the user for which it was generated all match, and the user is
    either logged in to Facebook or has granted an offline access permission.

    :param string: An authorization code.

    :rtype: mixed An access token exchanged for the authorization code, or
              false if an access token could not be generated.



_restserver
-----------

.. function:: _restserver()


    Invoke the old restserver.php endpoint.

    :param array: Method call object

    :rtype: mixed The decoded response object

    :throws: FacebookApiException 



isVideoPost
-----------

.. function:: isVideoPost()


    Return true if this is video post.

    :param string: The path
    :param string: The http method (default 'GET')

    :rtype: boolean true if this is video post



_graph
------

.. function:: _graph()


    Invoke the Graph API.

    :param string: The path (required)
    :param string: The http method (default 'GET')
    :param array: The query/post data

    :rtype: mixed The decoded response object

    :throws: FacebookApiException 



_oauthRequest
-------------

.. function:: _oauthRequest()


    Make a OAuth Request.

    :param string: The path (required)
    :param array: The query/post data

    :rtype: string The decoded response object

    :throws: FacebookApiException 



makeRequest
-----------

.. function:: makeRequest()


    Makes an HTTP request. This method can be overridden by subclasses if
    developers want to do fancier things or use something other than curl to
    make the request.

    :param string: The URL to make the request to
    :param array: The parameters to use for the POST body
    :param CurlHandler: Initialized curl handle

    :rtype: string The response text



parseSignedRequest
------------------

.. function:: parseSignedRequest()


    Parses a signed_request and validates the signature.

    :param string: A signed token

    :rtype: array The payload inside it or null if the sig is wrong



makeSignedRequest
-----------------

.. function:: makeSignedRequest()


    Makes a signed_request blob using the given data.

    :param array: data array.

    :rtype: string The signed request.



getApiUrl
---------

.. function:: getApiUrl()


    Build the URL for api given parameters.

    :param $method: the method name.

    :rtype: string The URL for the given parameters



getUrl
------

.. function:: getUrl()


    Build the URL for given domain alias, path and parameters.

    :param $name: The name of the domain
    :param $path: Optional path (without a leading slash)
    :param $params: Optional query parameters

    :rtype: string The URL for the given parameters



getHttpHost
-----------

.. function:: getHttpHost()



getHttpProtocol
---------------

.. function:: getHttpProtocol()



getBaseDomain
-------------

.. function:: getBaseDomain()


    Get the base domain used for the cookie.



getCurrentUrl
-------------

.. function:: getCurrentUrl()


    Returns the Current URL, stripping it of known FB parameters that should
    not persist.

    :rtype: string The current URL



shouldRetainParam
-----------------

.. function:: shouldRetainParam()


    Returns true if and only if the key or key/value pair should
    be retained as part of the query string.  This amounts to
    a brute-force search of the very small list of Facebook-specific
    params that should be stripped out.

    :param string: A key or key/value pair within a URL's query (e.g.
                    'foo=a', 'foo=', or 'foo'.

    :rtype: boolean 



throwAPIException
-----------------

.. function:: throwAPIException()


    Analyzes the supplied result to see if it was thrown
    because the access token is no longer valid.  If that is
    the case, then we destroy the session.

    :param $result: A record storing the error message returned
                     by a failed API call.



errorLog
--------

.. function:: errorLog()


    Prints to the error log if you aren't in command line mode.

    :param string: Log message



base64UrlDecode
---------------

.. function:: base64UrlDecode()


    Base64 encoding that doesn't need to be urlencode()ed.
    Exactly the same as base64_encode except it uses
      - instead of +
      _ instead of /
      No padded =

    :param string: base64UrlEncoded string

    :rtype: string 



base64UrlEncode
---------------

.. function:: base64UrlEncode()


    Base64 encoding that doesn't need to be urlencode()ed.
    Exactly the same as base64_encode except it uses
      - instead of +
      _ instead of /

    :param string: string

    :rtype: string base64Url encoded string



destroySession
--------------

.. function:: destroySession()


    Destroy the current session



getMetadataCookie
-----------------

.. function:: getMetadataCookie()


    Parses the metadata cookie that our Javascript API set

    :rtype: an array mapping key to value



isAllowedDomain
---------------

.. function:: isAllowedDomain()



endsWith
--------

.. function:: endsWith()



setPersistentData
-----------------

.. function:: setPersistentData()


    Stores the given ($key, $value) pair, so that future calls to
    getPersistentData($key) return $value. This call may be in another request.

    :param string: 
    :param array: 

    :rtype: void 



getPersistentData
-----------------

.. function:: getPersistentData()


    Get the data for $key, persisted by BaseFacebook::setPersistentData()

    :param string: The key of the data to retrieve
    :param boolean: The default value to return if $key is not found

    :rtype: mixed 



clearPersistentData
-------------------

.. function:: clearPersistentData()


    Clear the data with $key from the persistent storage

    :param string: 

    :rtype: void 



clearAllPersistentData
----------------------

.. function:: clearAllPersistentData()


    Clear all data from the persistent storage

    :rtype: void 





Constants
---------

VERSION
+++++++

Version.

SIGNED_REQUEST_ALGORITHM
++++++++++++++++++++++++

Signed Request Algorithm.

