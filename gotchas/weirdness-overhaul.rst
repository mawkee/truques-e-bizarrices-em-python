===================================
Gotcha - Probleminhas para resolver
===================================

::

    >>> ab = 1
    >>> ab += 1
    >>> ab
    2
    >>> def teste_1():
    ...     return ab + 1
    ...
    >>> def teste_2():
    ...     ab += 1
    ...     return ab
    ...
    >>> teste_1()
    3
    >>> teste_2()
    Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
    File "<stdin>", line 2, in teste_2
    UnboundLocalError: local variable 'ab' referenced before assignment


.. hidden-code-block:: python

    >>> from collections import Hashable
    >>> issubclass(list, object)
    True
    >>> issubclass(object, Hashable)
    True
    >>> issubclass(list, Hashable)
    False


.. hidden-code-block:: python

    >>> (False == False) in [False]
    False
    >>> False == (False in [False])
    False
    >>> False == False in [False]  # QUE?
    True

    >>> True is False == False
    False
    >>> False is False is False
    True

    >>> 1 > 0 < 1
    True
    >>> (1 > 0) < 1
    False
    >>> 1 > (0 < 1)
    False


.. hidden-code-block:: python

    # PARA O CONSOLE!
    >>> a, b = a[b] = {}, 5


.. hidden-code-block:: python

    >>> teste = 10
    >>> testе = 20
    >>> --teste
    10
    >>> ++testе
    20
