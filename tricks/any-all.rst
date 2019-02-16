=========================================
Truque - Any e All para clareza de código
=========================================

Para quem gosta de código legível, vamos além de `and` e `or`...

::

    >>> filters = [True, True, False]
    >>> if any(filters):
    ...     # Se qualquer das condições for verdadeira
    ...     ...
    >>> if all(filters):
    ...     # Se todas as condições forem verdadeiras
    ...     ...
    >>> if any(filter) and not all(filters):
    ...     # Se alguma condição for verdadeira, mas não todas
    ...     ...
