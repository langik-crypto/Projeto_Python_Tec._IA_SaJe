Conversor e Validador de Dados Climáticos de Manaus

Descrição:

Este projeto foi desenvolvido para a disciplina de Programação em Python e tem como objetivo processar registros climáticos simulados de uma estação meteorológica de Manaus.

O sistema recebe dados no formato:

32.5C,85%

Onde:

* O primeiro valor representa a temperatura em graus Celsius.
* O segundo valor representa a umidade relativa do ar em porcentagem.

O programa realiza a validação dos dados, identifica registros inválidos, converte temperaturas para Fahrenheit, classifica a sensação térmica e gera um resumo das condições climáticas observadas.


Funcionalidades:

* Leitura de registros climáticos.
* Parsing de strings para obtenção de temperatura e umidade.
* Validação de dados corrompidos ou fora das faixas aceitáveis.
* Conversão de temperatura de Celsius para Fahrenheit.
* Classificação da sensação térmica.
* Geração de relatório climático.
* Resumo estatístico do dia.



Tecnologias Utilizadas:

* Python 3



Estrutura dos Dados:

Exemplo de entrada:

32.5C,85%

Formato:

TemperaturaC,Umidade%

Exemplos válidos:

32.5C,85%
28C,70%
40C,95%

Exemplos inválidos:

50C,30%
30C,110%
abc



Como Executar:

1. Instale o Python 3.
2. Baixe ou clone este repositório.
3. Execute o arquivo principal:

python trabalho.py



Exemplo de Saída:

Temperatura: 32.5°C
Fahrenheit: 90.5°F
Umidade: 85%
Sensação: Muito Quente

Resumo do dia:
Registros válidos: 4
Registros inválidos: 2




Dupla: Jéssica Lange Miranda Barbosa e Sadrack Maia Jesus
Curso: Técnico em Inteligência Artificial
Disciplina: Programação em Python
