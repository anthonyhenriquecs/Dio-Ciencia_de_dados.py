# Dio-Ciencia_de_dados.py

while True:
    try:
        entrada = input("Digite a distância, diâmetro de Sauron e diâmetro de Saruman separados por espaços: ").split()

        if len(entrada) == 3:
            distancia = int(entrada[0])
            diametro1 = int(entrada[1])
            diametro2 = int(entrada[2])

            # Calcular o Índice de Comunicação Mágica (ICM)
            icm = distancia / (diametro1 + diametro2)

            print(f"Índice de Comunicação Mágica (ICM) {icm:.2f}")
            break
        else:
            print("Entrada inválida. Certifique-se de fornecer três valores separados por espaço.")
    except ValueError:
        print("Erro de valor. Certifique-se de fornecer valores numéricos.")
