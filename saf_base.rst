.. saf_base.php generated using docpx on 01/30/13 03:58pm


Class
*****

SAF_Base
========

Methods
-------

__construct
+++++++++++

.. function:: __construct()


    Constructor


    :rtype: void 



createSafVariableName
+++++++++++++++++++++

.. function:: createSafVariableName()


    Returns a SAF variable name in the form of "saf_APPID_key".


    :param string: the key name

    :rtype: string 



setSafPersistentData
++++++++++++++++++++

.. function:: setSafPersistentData()


    Sets a SAF session variable


    :param string: the key name
    :param string: the value

    :rtype: void 



getSafPersistentData
++++++++++++++++++++

.. function:: getSafPersistentData()


    Returns a SAF session variable


    :param string: the key name
    :param string: the default value to return

    :rtype: mixed 



clearSafPersistentData
++++++++++++++++++++++

.. function:: clearSafPersistentData()


    Unsets a SAF session variable


    :param string: the key name

    :rtype: void 



debug
+++++

.. function:: debug()


    Wrapper around an external class so we can do a simple check if the
    class (XS_Debug) is avaliable before we attempt to use its method.


    :param string: name, label, message
    :param var: a variable
    :param int: (1)log, (2)info, (3)warn, (4)error
    :param bool: log to text file

    :rtype: void 



