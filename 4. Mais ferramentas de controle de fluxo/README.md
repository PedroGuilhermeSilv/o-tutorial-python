## 4.1. Comandos if
- Provavelmente o mais conhecido comando de controle de fluxo é o if. Por exemplo:
```
>>> x = int(input("Please enter an integer: "))
Please enter an integer: 42
>>> if x < 0:
...     x = 0
...     print('Negative changed to zero')
... elif x == 0:
...     print('Zero')
... elif x == 1:
...     print('Single')
... else:
...     print('More')
...
```
- Pode haver zero ou mais partes elif, e a parte else é opcional. A palavra-chave ‘elif’ é uma abreviação para ‘else if’, e é útil para evitar indentação excessiva. Uma sequência if … elif … elif … substitui os comandos switch ou case, encontrados em outras linguagens.

## 4.2. Comandos for
- O comando for em Python é um pouco diferente do que costuma ser em C ou Pascal. Ao invés de sempre iterar sobre uma progressão aritmética de números (como no Pascal), ou permitir ao usuário definir o passo de iteração e a condição de parada (como C), o comando for do Python itera sobre os itens de qualquer sequência (seja uma lista ou uma string), na ordem que aparecem na sequência.
 
## 4.3. A função range()
- Se você precisa iterar sobre sequências numéricas, a função embutida range() é a resposta.

## 4.4. Comandos break e continue, e cláusula else, nos laços de repetição
- O comando break, como no C, sai imediatamente do laço de repetição mais interno, seja for ou while. Laços podem ter uma cláusula else, que é executada sempre que o laço se encerra por exaustão do iterável (no caso do for) ou quando a condição se torna falsa (no caso do while), mas nunca quando o laço é interrompido por um break.

## 4.5. Comandos pass
- O comando pass não faz nada. Pode ser usada quando a sintaxe exige um comando mas a semântica do programa não requer nenhuma ação.

## 4.6 Instruções match
- Uma instrução match pega uma expressão e compara seu valor com padrões sucessivos fornecidos como um ou mais blocos de case. Isso é superficialmente semelhante a uma instrução switch em C, Java ou JavaScript (e muitas outras linguagens), mas também pode extrair componentes (elementos de sequência ou atributos de objeto) do valor em variáveis, mas muito mais parecido com a correspondência de padrões em linguages como Rust ou Haskell. Observe o último bloco: o “nome da variável” _ atua como um curinga e nunca falha em corresponder. Se nenhum caso corresponder, nenhuma das ramificações será executada.
```
def http_error(status):
    match status:
        case 400|200:
            return "Bad request"
        case 404:
            return "Not found"
        case 418:
            return "I'm a teapot"
        case _:
            return "Something's wrong with the internet"
```