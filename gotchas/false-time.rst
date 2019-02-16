=========================================
Gotcha - Dois perdidos em uma noite falsa
=========================================

Por algum motivo, alguém achou que isso não era um bug...

::

    >>> import datetime
    >>> bool(datetime.time(0, 0))
    False
    >>> bool(datetime.time(0, 1))
    True
