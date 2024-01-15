# If e Else

Em Python, if e else são estruturas de controle de fluxo que permitem tomar decisões condicionais em um programa. Essas estruturas são fundamentais para controlar o fluxo de execução do código com base em condições específicas.

A sintaxe básica é a seguinte:

if condição:
    # Bloco de código a ser executado se a condição for verdadeira
else:
    # Bloco de código a ser executado se a condição for falsa

## Aqui está um exemplo em Markdown para ilustrar o uso de if e else em Python:

```python
# Exemplo de uso de if e else em Python

# Recebe um número do usuário
numero = int(input("Digite um número: "))

# Verifica se o número é positivo, negativo ou zero
if numero > 0:
    print("O número é positivo.")
elif numero < 0:
    print("O número é negativo.")
else:
    print("O número é zero.")


Neste exemplo:

1. O programa solicita ao usuário que insira um número.
2. A condição `if numero > 0:` verifica se o número é positivo.
3. Se a condição for verdadeira, o bloco de código dentro do `if` será executado, imprimindo "O número é positivo."
4. Se a condição não for verdadeira, o programa verifica a condição `elif numero < 0:` para determinar se o número é negativo.
5. Se a condição `elif` for verdadeira, o bloco de código dentro dela será executado, imprimindo "O número é negativo."
6. Se nenhuma das condições anteriores for verdadeira, o bloco de código dentro do `else` será executado, imprimindo "O número é zero."

Dessa forma, `if` e `else` são utilizados para controlar o fluxo do programa com base nas condições especificadas.


Vamos criar um simples projeto em Python que solicita ao usuário que adivinhe um número. O programa gerará um número aleatório e o usuário terá que tentar adivinhar. O programa dará dicas indicando se o número fornecido pelo usuário é maior, menor ou igual ao número gerado aleatoriamente. Aqui está um exemplo:

import random

def jogo_adivinhacao():
    # Gera um número aleatório entre 1 e 100
    numero_secreto = random.randint(1, 100)

    tentativas = 0
    max_tentativas = 5

    print("Bem-vindo ao Jogo de Adivinhação!")
    print("Tente adivinhar o número secreto entre 1 e 100.")

    while tentativas < max_tentativas:
        try:
            # Solicita ao usuário que insira um palpite
            palpite = int(input("Digite seu palpite: "))

            # Verifica se o palpite é igual ao número secreto
            if palpite == numero_secreto:
                print(f"Parabéns! Você acertou o número secreto {numero_secreto}!")
                break
            elif palpite < numero_secreto:
                print("Tente novamente. O número secreto é maior.")
            else:
                print("Tente novamente. O número secreto é menor.")

            tentativas += 1

        except ValueError:
            print("Por favor, digite um número válido.")

    if tentativas == max_tentativas:
        print(f"Fim de jogo! O número secreto era {numero_secreto}.")

# Chama a função principal
jogo_adivinhacao()


Neste exemplo:

Utilizamos a biblioteca random para gerar um número aleatório.
A função jogo_adivinhacao inicia o jogo, gerando um número aleatório e configurando o número máximo de tentativas.
Um loop while é utilizado para permitir que o usuário faça múltiplos palpites até acertar ou atingir o número máximo de tentativas.
Dentro do loop, usamos instruções if e else para comparar o palpite do usuário com o número secreto e fornecer dicas.
Se o usuário acertar, uma mensagem de parabéns é exibida. Se o número máximo de tentativas for atingido, uma mensagem informando o número secreto é exibida.
Este é apenas um exemplo simples, mas ilustra como as estruturas if e else podem ser utilizadas para criar lógica condicional em um programa Python.

Obs:Todos os projetos que fiz estarão no repositório " pythonprojects".

