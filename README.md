# o-tutorial-python

## 3. Uma introdução informal ao Python
1. Número
2. String
3. Lista

## 4. Mais ferramentas de controle de fluxo
1. Comandos if
2. Comandos for
3. A função range()
4. Comandos break e continue, e cláusula else, nos laços de repetição
5. Comandos pass



### Anotações:
## args e kwargs
- args vai tratar de todos argumentos não nomeados e o kwargs o inverso então eu posso receber em uma função esses parãmetros que serão desempacotados em tupla ou dicionário.

```
def func(*args,**kwargs):
    args
    kwargs.items()
func(1,nome="test")
```


#### Esta documentação é um resumo do livro [O Tutorial de Python](https://docs.python.org/pt-br/3.10/tutorial/introduction.html#lists)