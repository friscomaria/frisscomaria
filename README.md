def calcular_fatorial(n):
    if n == 0 or n == 1:
        return 1
    resultado = 1
    while n > 1:
        resultado *= n
        n -= 1
    return resultado

while True:
    try:
        numero = int(input("Digite um número para calcular o fatorial (ou digite '0' para sair): "))
        if numero == 0:
            break
        resultado = calcular_fatorial(numero)
        print(f'O fatorial de {numero} é {resultado}')
    except ValueError:
        print("Por favor, digite um número válido.")
