Aqui está um código simples em Python que solicita dois números do usuário, pergunta qual operação deseja realizar e, em seguida, realiza a operação com base na escolha:

python
Copiar código
# Solicitar ao usuário dois números
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

# Perguntar ao usuário qual operação deseja realizar
operacao = input("Escolha a operação (soma, subtração, multiplicação, divisão, exponenciação): ").lower()

# Usar estruturas condicionais para realizar a operação escolhida
if operacao == "soma":
    resultado = num1 + num2
    print(f"O resultado da soma é: {resultado}")

elif operacao == "subtração":
    resultado = num1 - num2
    print(f"O resultado da subtração é: {resultado}")

elif operacao == "multiplicação":
    resultado = num1 * num2
    print(f"O resultado da multiplicação é: {resultado}")

elif operacao == "divisão":
    if num2 != 0:
        resultado = num1 / num2
        print(f"O resultado da divisão é: {resultado}")
    else:
        print("Erro: Divisão por zero não é permitida!")

elif operacao == "exponenciação":
    resultado = num1 ** num2
    print(f"O resultado da exponenciação é: {resultado}")

else:
    print("Operação inválida! Por favor, escolha entre soma, subtração, multiplicação, divisão, ou exponenciação.")
Esse código utiliza if-elif-else para verificar a operação escolhida e realiza o cálculo de acordo com a escolha. Ele também inclui um tratamento de erro para a divisão por zero.







Você disse:
condicao if dentro de um for python
O ChatGPT disse:
ChatGPT
Usar a condição if dentro de um loop for em Python é bastante comum quando você deseja verificar uma condição para cada item em uma sequência (como listas, tuplas, strings, etc.). Aqui está um exemplo básico que ilustra como isso funciona:

Exemplo 1: Verificando números pares em uma lista
python
Copiar código
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Percorrer a lista com um for
for numero in numeros:
    # Verificar se o número é par
    if numero % 2 == 0:
        print(f"{numero} é par")
Exemplo 2: Verificando se palavras contêm a letra "a"
python
Copiar código
palavras = ["gato", "cachorro", "elefante", "abelha", "leão"]

# Percorrer a lista de palavras
for palavra in palavras:
    # Verificar se a palavra contém a letra 'a'
    if 'a' in palavra:
        print(f"A palavra '{palavra}' contém a letra 'a'")
Exemplo 3: Filtrar números maiores que 5
python
Copiar código
numeros = [2, 5, 8, 3, 9, 1, 7]

# Filtrar números maiores que 5
for numero in numeros:
    if numero > 5:
        print(f"{numero} é maior que 5")
Em todos esses exemplos, a condição if é usada dentro de um loop for para aplicar algum critério aos itens da lista.






