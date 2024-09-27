# Projeto
Questões Gupy feitas em Python

1- Questão:

indice = 13
soma = 0
k = 0

while k < indice:
    k += 1
    soma += k
    break

print(soma)

2- Questão:

def fibonacci(c):
    a, b = 0, 1
    while a <= c:
        if a == c:
            return True
        a, b = b, a + b
    return False

numero = int(input('Digite o número:'))

if fibonacci(numero):
    print(f"O número {numero} pertence à sequência de Fibonacci.")
else:
    print(f"O número {numero} não pertence à sequência de Fibonacci.")

3- Questão:

faturamento = [
	{
		"dia": 1,
		"valor": 22174.1664
	},
	{
		"dia": 2,
		"valor": 24537.6698
	},
	{
		"dia": 3,
		"valor": 26139.6134
	},
	{
		"dia": 6,
		"valor": 26742.6612
	},
	{
		"dia": 8,
		"valor": 42889.2258
	},
	{
		"dia": 9,
		"valor": 46251.174
	},
	{
		"dia": 10,
		"valor": 11191.4722
	},
	{
		"dia": 13,
		"valor": 3847.4823
	},
	{
		"dia": 14,
		"valor": 373.7838
	},
	{
		"dia": 15,
		"valor": 2659.7563
	},
	{
		"dia": 16,
		"valor": 48924.2448
	},
	{
		"dia": 17,
		"valor": 18419.2614
	},
	{
		"dia": 20,
		"valor": 35240.1826
	},
	{
		"dia": 21,
		"valor": 43829.1667
	},
	{
		"dia": 22,
		"valor": 18235.6852
	},
	{
		"dia": 23,
		"valor": 4355.0662
	},
	{
		"dia": 24,
		"valor": 13327.1025
	},
	{
		"dia": 27,
		"valor": 25681.8318
	},
	{
		"dia": 28,
		"valor": 1718.1221
	},
	{
		"dia": 29,
		"valor": 13220.495
	},
	{
		"dia": 30,
		"valor": 8414.61
    }
]

valores = []
for dia in faturamento:
    valores.append(dia["valor"]);

menor_faturamento = min(valores);
maior_faturamento = max(valores);

print(f"Menor valor de faturamento em um dia do mês: {menor_faturamento}")
print(f"Maior valor de faturamento em um dia do mês: {maior_faturamento}")


4- Questão:

 faturamento = {
    "SP": 67836.43,
    "RJ": 36678.66,
    "MG": 29229.88,
    "ES": 27165.48,
    "Outros": 19849.53
}

total_faturamento = sum(faturamento.values())

for estado, valor in faturamento.items():
    percentual = (valor / total_faturamento) * 100
    print(f"{estado}: {percentual:.2f}%")

5- Questão: 

inversao = input('Digite a palavra:')

nome_inversao = []

for i in range(len(inversao) - 1, -1, -1):
    nome_inversao.append(inversao[i])

print(f"String invertida: {nome_inversao}")
