=================================================
Truque - AND e OR retornam objetos, não booleanos
=================================================

Em Python, o `and` e o `or` retornam valores de acordo com a seguinte regra:
- `a and b` retorna o último valor verdadeiro, ou o primeiro falso
- `a or b` retorna o primeiro valor verdadeiro, ou o último falso

Isso permite algumas construções interessantes

::

    >>> def minha_funcao_bizarra(obj, nome=None, bloco=None):
    >>>     obj.nome = nome or "Nome padrão"
    >>>     obj.bloco = bloco or 2


PS: Cuidado ao usar!
