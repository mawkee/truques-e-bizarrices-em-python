============================
Gotcha - Argumentos mutáveis
============================

Dicionários em Python podem fazer unpacking em um segundo dicionário
::

    >>> def funcionezita(pessoas=[]):
    ...     pessoas.append("Mawkee")
    ...     return pessoas

    >>> funcionezita()
    ['Mawkee']
    >>> funcionezita()
    # ??


.. hidden-code-block:: python
    :starthidden: True

    >>> funcionezita()
    ["Mawkee"]
    >>> funcionezita()
    ['Mawkee', 'Mawkee']
    >>> funcionezita()
    ['Mawkee', 'Mawkee', 'Mawkee']


.. hidden-code-block:: python
    :starthidden: True

    # Use sempre None para isso
    >>> def funcionezita(pessoas=None):
    ...     if not pessoas:
    ...         pessoas = []
    ...     pessoas.append("Mawkee")
    ...     return pessoas
