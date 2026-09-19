# entregavel-2

numeros = []

for posicao in range(5):
	numero = float(input(f"Introduza o {posicao + 1}.º número: "))
	numeros.append(numero)

soma = 0
maior = numeros[0]
menor = numeros[0]

for numero in numeros:
	soma += numero

	if numero > maior:
		maior = numero

	if numero < menor:
		menor = numero

media = soma / len(numeros)

print(f"Soma: {soma}")
print(f"Média: {media}")
print(f"Maior valor: {maior}")
print(f"Menor valor: {menor}")



idade = inteiro(entrada("Digite a idade do cliente: "))
renda = flutuador(entrada("Digite a renda mensal do cliente: R$ "))
se idade < 0 ou renda < 0:
	imprimir("Idade e renda devem ser valores positivos.")
elif renda < 2000:
	imprimir("Categoria: Bronze")
elif renda < 5000:
	imprimir("Categoria: Prata")
elif renda < 10000:
	imprimir("Categoria: Ouro")
outro:
	imprimir("Categoria: Diamante")





  imprimir("Menu de operações matemáticas")
imprimir("1 - Soma")
imprimir("2 - Subinto")
imprimir("3 - Multiplicação")
imprimir("4 - Divisão")
opcao = entrada("Escolha uma operação: ")
se opcao em("1","2","3","4"):
	primeiro_número = flutuador(entrada("Apresenta o primeiro número:"))
	segundo_numero = flutuador(entrada("Apresenta o segundo número:"))
	corresponder opcao:
		caso "1":
			resultado = primeiro_número + segundo_numero
		caso "2":
			resultado = primeiro_número - segundo_numero
		caso "3":
			resultado = primeiro_número * segundo_numero
		caso "4":
			se segundo_numero == 0:
				resultado = Nenhum
				imprimir("Não é possível dividir por zero.")
			outro:
				resultado = primeiro_número / segundo_numero
	se resultado é não Nenhum:
		imprimir(f"Resultado:{resultado}")
outro:
	imprimir("Opção inválida.")







  palavra_passe_correta = "python123"
esforço = 0
acesso_autorizado = Falso
enquanto esforço < 3 e não acesso_autorizado:
	palavra_passe = entrada("Introduza a palavra-passe: ")
	esforço += 1
	se palavra_passe == palavra_passe_correta:
		acesso_autorizado = Verdadeiro
		imprimir("Acesso autorizado.")
	outro:
		_restantes = 3 - esforço
		se _restantes > 0:
			imprimir(f"Palavra-passe incorreto. Restam{_restantes}tentativa(s).")
se não acesso_autorizado:
	imprimir("Acesso bloqueado após 3 tentativas incorretas.")
