===============================
Truque - Combinando Dicionários
===============================

Dicionários em Python podem fazer unpacking em um segundo dicionário
::

    >>> x = {'a': 10, 'b': 20}
    >>> y = {'b': 30, 'd': 40}
    >>> z = {**x, **y}
    >>> z
    {'a': 10, 'b': 30, 'd': 40}

    >>> z = {**y, **x}
    >>> z
    {'b': 20, 'd': 40, 'a': 10}
