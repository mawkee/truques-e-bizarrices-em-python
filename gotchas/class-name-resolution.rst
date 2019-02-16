===================================================
Gotcha - Resolução de nomes ignora escopo da classe
===================================================


::

    >>> x = 23
    >>> class Pontos:
    ...     x = 42
    ...     y = [x for i in range(10)]
    >>> print(Pontos.y[0])
    23


(PEP 227)
