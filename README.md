# mamdani-inference

Mamdani

Veículo com 5 marchas

Definição das variáveis de entrada:

	1. Velocidade - baixa, média e alta. (Km/h)
		0-40 -> baixa
		30-90 -> média
		80-160 -> alta

	2. Marcha - baixa, média e alta. (Número da marcha)
		1,3 -> baixa
		2,3,4 -> média
		3,4,5 -> alta

	3. Inclinação - baixa, média e alta. (Em graus)
		0,10 -> baixa
		5,20 -> média
		15,30 -> alta

Definição da variável de saída

	1. Consumo de combustível - baixo, médio e alto. (Litros a cada 100 km)
		0,10 -> baixo
		8,16 -> médio
		14,100 -> alto
		

Base de Conhecimento - Regras Fuzzy

	1. Se a Velocidade é Baixa E a Marcha é Baixa E a Inclinação é Leve, ENTÃO o Consumo é Baixo.
	2. Se a Velocidade é Baixa E a Marcha é Baixa E a Inclinação é Moderada, ENTÃO o Consumo é Médio.
	3. Se a Velocidade é Baixa E a Marcha é Baixa E a Inclinação é Acentuada, ENTÃO o Consumo é Alto.

	4. Se a Velocidade é Média E a Marcha é Média E a Inclinação é Leve, ENTÃO o Consumo é Médio.
	5. Se a Velocidade é Média E a Marcha é Média E a Inclinação é Moderada, ENTÃO o Consumo é Alto.

	6. Se a Velocidade é Alta E a Marcha é Média E a Inclinação é Leve, ENTÃO o Consumo é Alto.
	7. Se a Velocidade é Alta E a Marcha é Média E a Inclinação é Moderada, ENTÃO o Consumo é Alto.

	8. Se a Velocidade é Alta E a Marcha é Alta E a Inclinação é Leve, ENTÃO o Consumo é Baixo.
	9. Se a Velocidade é Alta E a Marcha é Alta E a Inclinação é Moderada, ENTÃO o Consumo é Médio.