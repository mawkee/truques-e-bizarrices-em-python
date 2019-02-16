==================================================
Truque - Ordenação por .sort ou sorted() é estável
==================================================

No Python, a ordenação através de `sorted()` ou `.sort()` é garantida como sendo
estável; é perfeitamente _pythonico_ que se ordene uma lista duas vezes, para chegar
ao resultado final desejado

::

    >>> data = [('red', 1), ('blue', 1), ('red', 2), ('blue', 2)]
    >>> sorted(data, key=itemgetter(0))
    [('blue', 1), ('blue', 2), ('red', 1), ('red', 2)]

(da documentação oficial)
