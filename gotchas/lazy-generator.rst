====================================================
Gotcha - Lazy eval nem sempre age de forma intuitiva
====================================================

::

    >>> a = [1, 2, 3]
    >>> g = (i for i in a if a.count(i) > 0)
    >>> a = [3, 4, 5]
    >>> list(g)
    ??????


.. hidden-code-block:: python

    >>> a = [1, 2, 3]
    >>> g = (i for i in a if a.count(i) > 0)
    >>> a = [3, 4, 5]
    >>> list(g)
    [3]
