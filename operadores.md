1️⃣ **Operadores Aritméticos**

| Operador | Descrição              | Exemplo      | Resultado |
|----------|-----------------------|--------------|-----------|
| `+`      | Adição                | `5 + 3`      | `8`       |
| `-`      | Subtração             | `5 - 3`      | `2`       |
| `*`      | Multiplicação         | `5 * 3`      | `15`      |
| `/`      | Divisão (resultado float) | `5 / 2`  | `2.5`     |
| `%`      | Módulo (resto da divisão) | `5 % 2`  | `1`       |
| `//`     | Divisão inteira           | `5 // 2` | `2`       |
| `**`     | Potência                  | `5 ** 2` | `25`      |


2️⃣ **Operadores de Comparação**

| Operador | Descrição                    | Exemplo     | Resultado |
|----------|-----------------------------|-------------|-----------|
| `==`     | Igual a                     | `5 == 5`    | `True`    |
| `!=`     | Diferente de                | `5 != 3`    | `True`    |
| `>`      | Maior que                   | `5 > 3`     | `True`    |
| `<`      | Menor que                   | `3 < 5`     | `True`    |

3️⃣ **Operadores Lógicos**

| Operador | Descrição                   | Exemplo                   | Resultado |
|----------|----------------------------|---------------------------|-----------|
| `and`    | E lógico (ambos True)       | `True and False`          | `False`   |
| `or`     | Ou lógico (pelo menos um True) | `True or False`         | `True`    |
| `not`    | Negação lógica (inverte)    | `not True`                | `False`   |

4️⃣ **Operadores de Atribuição**

| Operador | Descrição                    | Exemplo              | Resultado      |
|----------|-----------------------------|----------------------|----------------|
| `=`      | Atribuição simples           | `x = 5`              | `x` recebe 5   |
| `+=`     | Soma e atribui (incrementa)  | `x += 3` (equivale a `x = x + 3`) | `x` aumenta 3 |
| `-=`     | Subtrai e atribui (decrementa) | `x -= 2` (equivale a `x = x - 2`) | `x` diminui 2 |

5️⃣ Outros Operadores Comuns

| Operador | Descrição                                             | Exemplo              | Resultado      |
| -------- | ----------------------------------------------------- | -------------------- | -------------- |
| `in`     | Verifica se um valor está em uma sequência            | `3 in [1, 2, 3]`     | `True`         |
| `not in` | Verifica se um valor **não** está em uma sequência    | `4 not in [1, 2, 3]` | `True`         |
| `is`     | Verifica se duas variáveis referenciam o mesmo objeto | `a is b`             | `True`/`False` |

---

**Ordem de Precedência dos Operadores**

A ordem em que Python avalia os operadores pode mudar o resultado de uma expressão. Por exemplo:

```
resultado = 2 + 3 * 4   # resultado é 14, pois * tem precedência sobre +
```

Use parênteses para garantir a ordem desejada:

```
resultado = (2 + 3) * 4  # resultado é 20
```
