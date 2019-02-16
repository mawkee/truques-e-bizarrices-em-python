================================
Truque - For e Try permitem else
================================

No For, o else é executado quando não houver um `break`
=======================================================

::

    >>> for a in range(2, num):
    >>>     if num % a == 0:
    >>>         print("Não é primo")
    >>>         break
    >>>     else:
    >>>         print("É primo")


No Try, o else é executado quando não houver uma exception
==========================================================

::

    >>> try:
    >>>     next_number = n / previous_number
    >>> except ZeroDivisionError:
    >>>     DestroyTheUniverse()
    >>>     next_number = float('infinity')
    >>> else:
    >>>     valid_numbers.append(next_number)
    >>> finally:
    >>>     return next_number


**BONUS ROUND!!!!**
===================

Cuidado com a clausula `finally`, pois ela é executada mesmo depois de um `return`!
