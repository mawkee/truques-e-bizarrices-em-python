=================================================
Gotcha - Comparação de identidades entre inteiros
=================================================

::

    >>> a = 1
    >>> b = 1
    >>> a is b
    True
    >>> a = 100
    >>> b = 100
    >>> a is b
    True
    >>> a = 1000
    >>> b = 1000
    >>> a is b
    False


**?!?!?!?!?**

.. hidden-code-block:: python

    >>> # `is` não deve ser usado para comparações de valores
    >>> a == b
    True
