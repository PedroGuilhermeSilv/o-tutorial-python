## String
- Uma string é imutável.
- Uma string pode ser tratada como lista:
    - podemos acessar uma letra esperficia passando o índice desejado ou o intervalo desejado:
    ```
    >>> word = 'Python'
    >>> word[0]  # character in position 0
    'P'
    >>> word[0:2]  # characters from position 0 (included) to 2 (excluded)
    'Py'

    ```
## Listas
- A mais versátil é list (lista), que pode ser escrita como uma lista de valores (itens) separados por vírgula, entre colchetes.
- Como strings, listas pode ser indexados e fatiados. Todas as operações de fatiamento devolvem uma nova lista contendo os elementos solicitados. Isso significa que o seguinte fatiamento devolve uma cópia rasa da lista:
```
>>> squares[0]  # indexing returns the item
1
>>> squares[-1]
25


```
- As listas também suportam operações como concatenação:
```
>>> squares + [36, 49, 64, 81, 100]
[1, 4, 9, 16, 25, 36, 49, 64, 81, 100]

```
- Você também pode adicionar novos itens no final da lista, usando o método append() (estudaremos mais a respeito dos métodos posteriormente):
```
>>> cubes.append(216)
```



