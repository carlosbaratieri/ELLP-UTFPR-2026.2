# Lista de Exercícios — Python

## Lote 1 — Entrada, saída e operações matemáticas

1. Faça um programa que leia um número inteiro e o imprima.

```python
numero = int(input("Digite um número inteiro: "))

print("Número digitado:", numero)
```


2. Faça um programa que leia um número real e o imprima.

3. Peça ao usuário para digitar três valores inteiros e imprima a soma deles.

4. Leia um número real e imprima o resultado do quadrado desse número.

5. Leia um número real e imprima a quinta parte deste número.

6. Leia uma temperatura em graus Celsius e apresente-a convertida em graus Fahrenheit. A fórmula de conversão é: F = C * (9.0/5.0) + 32.0, sendo F a temperatura em Fahrenheit e C a temperatura em Celsius.

## Lote 2 — Estruturas condicionais

1. Faça um programa que receba dois números e mostre qual deles é o maior.

```python
numero1 = float(input("Digite o primeiro número: "))
numero2 = float(input("Digite o segundo número: "))

if numero1 > numero2:
    print("O maior número é:", numero1)
elif numero2 > numero1:
    print("O maior número é:", numero2)
else:
    print("Os números são iguais")
```


2. Leia um número fornecido pelo usuário. Se esse número for positivo, calcule a raiz quadrada do número. Se o número for negativo, mostre uma mensagem dizendo que o número é inválido.

3. Leia um número real. Se o número for positivo, imprima a raiz quadrada. Do contrário, imprima o número ao quadrado.

4. Faça um programa que leia um número e, caso ele seja positivo, calcule e mostre:
   - O número digitado ao quadrado.
   - A raiz quadrada do número digitado.

5. Faça um programa que receba um número inteiro e verifique se este número é par ou ímpar.

6. Escreva um programa que, dados dois números inteiros, mostre na tela o maior deles, assim como a diferença existente entre ambos.
