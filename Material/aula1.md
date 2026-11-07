# Introdução à Programação com Python

## 1. Conceitos básicos

### 1.1 O que é programação?

Programação é o processo de criar instruções para que um computador execute determinadas tarefas. Essas instruções são escritas utilizando linguagens de programação.

### 1.2 O que é Python?

Python é uma linguagem de programação de alto nível, conhecida por sua sintaxe simples e fácil leitura.

### 1.3 Primeiro programa

O primeiro contato com uma linguagem de programação geralmente é feito por meio de um programa que exibe a mensagem "Olá, mundo!".

Em Python, utilizamos a função `print()` para exibir informações na tela:

```python
print("Olá, mundo!")
```

## 2. Variáveis e tipos de dados

### 2.1 O que são variáveis?

Variáveis são espaços utilizados para armazenar informações na memória do computador. Cada variável possui um nome e pode guardar diferentes valores, como números, textos e valores booleanos (Verdadeiro ou Falso).

### 2.2 Atribuição de valores

Em Python, utilizamos o operador `=` para atribuir um valor a uma variável.

Exemplo:

```python
nome = "Pedro"
idade = 10
altura = 1.45
```

Nesse exemplo, criamos três variáveis e armazenamos diferentes informações em cada uma delas.

### 2.3 Tipos de dados

Os tipos de dados definem quais informações podem ser armazenadas em uma variável.

- **Inteiros (`int`):** representam números inteiros, positivos ou negativos.

```python
idade = 10
```

- **Reais (`float`):** representam números com casas decimais.

```python
altura = 1.45
```

- **Textos (`str`):** representam sequências de caracteres, escritas entre aspas.

```python
nome = "Pedro"
```

- **Booleanos (`bool`):** representam valores lógicos, que podem ser `True` (verdadeiro) ou `False` (falso).

```python
aprovado = True
```

### 2.4 Conversão de tipos

Em Python, podemos converter valores de um tipo para outro utilizando funções específicas:

- `int()`: converte um valor para inteiro.
- `float()`: converte um valor para real.
- `str()`: converte um valor para texto.

Exemplo:

```python
numero = "10"
numero = int(numero)

altura = "1.75"
altura = float(altura)

idade = 15
idade = str(idade)
```

A conversão de tipos é importante quando precisamos trabalhar com valores que foram recebidos ou armazenados em formatos diferentes.

## 3. Operadores e expressões

### 3.1 Operadores aritméticos

Os operadores aritméticos são utilizados para realizar cálculos matemáticos. Em Python, podemos utilizar:

| Operador | Operação | Exemplo | Resultado |
|---|---|---|---|
| `+` | Adição | `5 + 3` | `8` |
| `-` | Subtração | `5 - 3` | `2` |
| `*` | Multiplicação | `5 * 3` | `15` |
| `/` | Divisão | `6 / 3` | `2.0` |
| `//` | Divisão inteira | `7 // 2` | `3` |
| `%` | Resto da divisão | `7 % 2` | `1` |
| `**` | Potenciação | `2 ** 3` | `8` |

Exemplo:

```python
numero1 = 10
numero2 = 5

soma = numero1 + numero2
print(soma)
```

**Saída:**

```text
15
```

### 3.2 Operadores relacionais

Os operadores relacionais são utilizados para comparar valores. O resultado de uma comparação sempre será `True` (verdadeiro) ou `False` (falso).

| Operador | Significado | Exemplo |
|---|---|---|
| `==` | Igual a | `5 == 5` |
| `!=` | Diferente de | `5 != 3` |
| `>` | Maior que | `5 > 3` |
| `<` | Menor que | `3 < 5` |
| `>=` | Maior ou igual a | `5 >= 5` |
| `<=` | Menor ou igual a | `3 <= 5` |

Exemplo:

```python
idade = 12

print(idade >= 10)
```

**Saída:**

```text
True
```

### 3.3 Operadores lógicos

Os operadores lógicos permitem combinar condições ou inverter seus resultados.

- `and`: retorna verdadeiro quando todas as condições são verdadeiras.
- `or`: retorna verdadeiro quando pelo menos uma condição é verdadeira.
- `not`: inverte o resultado de uma condição.

Exemplo com `and`:

```python
idade = 12

print(idade >= 10 and idade <= 15)
```

**Saída:**

```text
True
```

Nesse exemplo, as duas condições são verdadeiras.

### 3.4 Expressões matemáticas e precedência de operadores

Uma expressão matemática é uma combinação de números, variáveis e operadores que produz um resultado.

Em Python, assim como na matemática, existe uma ordem de prioridade para realizar as operações:

1. Parênteses `()`.
2. Potenciação `**`.
3. Multiplicação, divisão e operações relacionadas (`*`, `/`, `//`, `%`).
4. Adição e subtração (`+`, `-`).

Exemplo:

```python
resultado = 2 + 3 * 4
print(resultado)
```

**Saída:**

```text
14
```

A multiplicação é realizada primeiro. Se quisermos realizar a adição antes, podemos utilizar parênteses:

```python
resultado = (2 + 3) * 4
print(resultado)
```

**Saída:**

```text
20
```

---

## 4. Entrada e saída de dados

### 4.1 Exibição de informações com `print()`

A função `print()` permite mostrar informações na tela, como textos, números e valores armazenados em variáveis.

Exemplo:

```python
nome = "Ana"
idade = 10

print("Nome:", nome)
print("Idade:", idade)
```

**Saída:**

```text
Nome: Ana
Idade: 10
```

### 4.2 Leitura de informações com `input()`

A função `input()` permite que o usuário digite informações durante a execução do programa.

Exemplo:

```python
nome = input("Digite seu nome: ")
print("Olá,", nome)
```

**Exemplo de execução:**

```text
Digite seu nome: Ana
Olá, Ana
```

### 4.3 Conversão de dados recebidos

Por padrão, a função `input()` recebe as informações como texto (`str`).

Por isso, quando precisamos realizar cálculos com os valores digitados, devemos convertê-los para o tipo adequado.

Exemplo:

```python
idade = int(input("Digite sua idade: "))
altura = float(input("Digite sua altura: "))

print("Idade:", idade)
print("Altura:", altura)
```

Nesse exemplo, utilizamos `int()` para receber um número inteiro e `float()` para receber um número com casas decimais.

### 4.4 Exibição de resultados

Depois de receber informações e realizar operações, podemos utilizar `print()` para apresentar os resultados ao usuário.

Exemplo:

```python
numero1 = float(input("Digite o primeiro número: "))
numero2 = float(input("Digite o segundo número: "))

soma = numero1 + numero2

print("O resultado da soma é:", soma)
```

**Exemplo de execução:**

```text
Digite o primeiro número: 10
Digite o segundo número: 5
O resultado da soma é: 15.0
```

Dessa forma, podemos criar programas que recebem informações, realizam cálculos e apresentam os resultados.

## 5. Estruturas condicionais

As estruturas condicionais permitem que um programa tome decisões. Com elas, podemos executar diferentes instruções dependendo de uma condição.

Por exemplo, podemos criar um programa que verifica se uma pessoa tem idade suficiente para participar de uma atividade.

### 5.1 Tomada de decisões

Uma condição é uma pergunta que pode ter apenas dois resultados: verdadeiro (`True`) ou falso (`False`).

Exemplo:

```python
idade = 12

print(idade >= 10)
```

**Saída:**

```text
True
```

Como a idade é maior ou igual a 10, o resultado da comparação é verdadeiro.

### 5.2 Estrutura `if`

A estrutura `if` permite executar um trecho de código somente quando uma condição é verdadeira.

Exemplo:

```python
idade = 12

if idade >= 10:
    print("Você pode participar!")
```

**Saída:**

```text
Você pode participar!
```

Se a condição for falsa, o código dentro do `if` não será executado.

### 5.3 Estrutura `if/else`

A estrutura `if/else` permite escolher entre dois caminhos: um quando a condição é verdadeira e outro quando é falsa.

Exemplo:

```python
idade = 8

if idade >= 10:
    print("Você pode participar!")
else:
    print("Você ainda não tem idade suficiente.")
```

**Saída:**

```text
Você ainda não tem idade suficiente.
```

### 5.4 Estrutura `if/elif/else`

A estrutura `elif` permite verificar outras condições quando as anteriores são falsas. Podemos utilizar quantos `elif` forem necessários.

Exemplo:

```python
nota = 8

if nota >= 9:
    print("Excelente!")
elif nota >= 7:
    print("Muito bem!")
elif nota >= 5:
    print("Você está quase lá!")
else:
    print("Precisa estudar mais!")
```

**Saída:**

```text
Muito bem!
```

### 5.5 Condicionais aninhadas

Condicionais aninhadas são estruturas condicionais colocadas dentro de outras estruturas condicionais. Elas permitem realizar verificações adicionais.

Exemplo:

```python
idade = 12
acompanhado = True

if idade >= 12:
    if acompanhado:
        print("Entrada permitida!")
    else:
        print("É necessário estar acompanhado.")
else:
    print("Idade insuficiente.")
```

**Saída:**

```text
Entrada permitida!
```

Nesse exemplo, primeiro verificamos a idade. Se ela for suficiente, verificamos se a pessoa está acompanhada.

**Importante:** em Python, a indentação (espaços no início da linha) é obrigatória para indicar quais instruções pertencem a cada estrutura condicional.
