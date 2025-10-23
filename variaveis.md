1️⃣ **Variáveis**

Variáveis são "caixinhas" onde a gente armazena valores para usar depois. Em Python, você pode criar uma variável simplesmente dando um nome para ela e atribuindo um valor.
Não precisa declarar o tipo explicitamente, Python entende automaticamente.

**Regras para nomes de variáveis:**

- Uma variável deve iniciar com uma letra ou um caracter underscore (_)
- Uma variável não pode começar com um número
- O nome de uma variável pode conter apenas caracteres alpha-numéricos e underscores (A-z, 0-9, e _)
- Nomes de variáveis são case sensitive (idade, Idade e IDADE são três variáveis diferentes)

**Reatribuição e tipagem dinâmica**

Você pode mudar o valor de uma variável quando quiser:

```
x = 5
x = 10  # Agora x vale 10
```

E o tipo da variável também pode mudar durante o programa:

```
var = 10      # int
var = "texto" # agora é string
```

**Boas práticas para nomes de variáveis**

- Use nomes significativos que expliquem o que a variável representa (ex: idade em vez de i)

- Use snake_case para nomes compostos, ou seja, letras minúsculas separadas por underscore (numero_inteiro)

- Evite nomes muito curtos ou confusos

**Variáveis múltiplas na mesma linha**

Você pode criar ou atribuir valores para várias variáveis de uma vez:

```
a, b, c = 1, 2, 3
```

**Constantes**

Python não tem constantes de verdade, mas por convenção usamos nomes em maiúsculas para indicar valores que não devem mudar:

```
PI = 3.14159
```

2️⃣ **Tipos de variáveis**

| Tipo       | Descrição                        | Exemplo                                 |
| ---------- | -------------------------------- | --------------------------------------- |
| `int`      | Número inteiro                   | `idade = 30`                            |
| `float`    | Número decimal (ponto flutuante) | `altura = 1.75`                         |
| `str`      | Texto (string)                   | `nome = "Maria"`                        |
| `bool`     | Booleano (verdadeiro ou falso)   | `estudando = True`                      |
| `list`     | Lista (coleção ordenada)         | `numeros = [1, 2, 3]`                   |
| `tuple`    | Tupla (lista imutável)           | `ponto = (10, 20)`                      |
| `dict`     | Dicionário (pares chave-valor)   | `pessoa = {"nome": "Ana", "idade": 25}` |
| `set`      | Conjunto (valores únicos)        | `conjunto = {1, 2, 3}`                  |
| `NoneType` | Representa ausência de valor     | `x = None`                              |

```
# int
idade = 28

# float
temperatura = 36.6

# str
cidade = "São Paulo"

# bool
verdadeiro = True
falso = False

# list
frutas = ["maçã", "banana", "laranja"]

# tuple
coordenadas = (10.0, 20.0)

# dict
carro = {"marca": "Ford", "ano": 2020}

# set
numeros = {1, 2, 3, 4}

# NoneType
resultado = None
```

3️⃣ **Uso das aspas em Python (strings)**

Para criar textos (strings), usamos aspas para delimitar o começo e o fim do texto.

Você pode usar:

- Aspas simples: 'texto'

- Aspas duplas: "texto"

- Aspas triplas simples: '''texto''' (para textos em várias linhas)

- Aspas triplas duplas: """texto""" (também para multilinhas)

Exemplos e dicas:

```
nome = 'João'                   # aspas simples
frase = "Python é ótimo!"       # aspas duplas

# Aspas simples dentro de aspas duplas (sem precisar escapar)
fala = "Ela disse: 'Olá!'"

# Aspas duplas dentro de aspas simples (sem precisar escapar)
resposta = 'Ele respondeu: "Oi!"'

# Escapando aspas com barra invertida \
texto = 'Ela disse: \'Tudo bem?\''

# Strings multilinhas
texto_multilinha = '''Linha 1
Linha 2
Linha 3'''
```

4️⃣ Tipos numéricos e operações básicas

Python trabalha com:

- int: números inteiros (ex: 10, -5)

- float: números decimais (ex: 3.14, -0.5)

- complex: números complexos (ex: 3 + 4j)

Operações comuns:
  
```
a = 10
b = 3

print(a + b)  # soma: 13
print(a - b)  # subtração: 7
print(a * b)  # multiplicação: 30
print(a / b)  # divisão: 3.3333333333333335 (float)
print(a // b) # divisão inteira: 3
print(a % b)  # resto da divisão: 1
print(a ** b) # potência: 10^3 = 1000
```
