# Exercicio2_Paython
Avaliação de Veiculos - Catgoria, Peso e Qtd Pessoas

INSTRUÇÕES DO PROJETO
Desenvolva um código que utilize as seguintes características de um veículo:
- Quantidade de rodas;
- Peso bruto em quilogramas;
- Quantidade de pessoas no veículo.

Com essas informações, o programa mostrará qual é a melhor categoria de habilitação para o veículo informado a partir das condições:
A: Veículos com duas ou três rodas;
B: Veículos com quatro rodas, que acomodam até oito pessoas e seu peso é de até 3500 kg;
C: Veículos com quatro rodas ou mais e com peso entre 3500 e 6000 kg;
D: Veículos com quatro rodas ou mais e que acomodam mais de oito pessoas; E: Veículos com quatro rodas ou mais e com mais de 6000 kg.

qtd_rodas = int (input ("Digite quantas rodas seu veículo possui: "))
peso_total = float (input ("Digite o peso total do seu veículo (kg): "))
qtd_pessoas = int (input ("Digite quantas pessoas cabem no seu veículo: "))

categoria = categoria_habilitacao(qtd_rodas, peso_total, qtd_pessoas)

if(qtd_rodas == 2 or qtd_rodas ==3):{
    print("Categoria A")
}
elif(qtd_rodas > 3 and peso_total <= 3500 and qtd_pessoas <= 8):{
    print("Categoria B")
}
elif(qtd_rodas >= 4 and peso_total > 3500 and peso_total <= 6000 ):{
    print("Categoria C")
}
elif(qtd_rodas >= 4 and qtd_pessoas > 8 and peso_total ):{
    print("Categoria D")
}
elif(qtd_rodas >= 4 and peso_total > 6000):{
    print("Categoria E")
}
else:{
    print("Categoria não definida!")
}

