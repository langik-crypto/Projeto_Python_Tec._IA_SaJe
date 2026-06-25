# 🌦️ Conversor e Validador de Dados Climáticos de Manaus

## 📖 Descrição

Este projeto foi desenvolvido para o Componente Curricular de **Programação em
Python** e tem como objetivo processar registros climáticos simulados de
uma estação meteorológica de Manaus.

O sistema recebe dados no seguinte formato:

``` text
32.5C,85%
```

Onde:

-   **Temperatura** em graus Celsius (`°C`);
-   **Umidade relativa do ar** em porcentagem (`%`).

O programa realiza a validação dos dados, identifica registros
inválidos, converte temperaturas para Fahrenheit, classifica a sensação
térmica e gera um resumo das condições climáticas observadas.

------------------------------------------------------------------------

## 🚀 Funcionalidades

-   Leitura de registros climáticos;
-   Parsing de strings para obtenção de temperatura e umidade;
-   Validação de dados corrompidos ou fora das faixas aceitáveis;
-   Conversão de temperatura de Celsius para Fahrenheit;
-   Classificação da sensação térmica;
-   Geração de relatório climático;
-   Resumo estatístico dos registros processados.

------------------------------------------------------------------------

## 🛠️ Tecnologias Utilizadas

-   Python 3

------------------------------------------------------------------------

## 📂 Estrutura dos Dados

### Formato da entrada

``` text
TemperaturaC,Umidade%
```

### Exemplo

``` text
32.5C,85%
```

### Exemplos de registros válidos

``` text
32.5C,85%
28C,70%
40C,95%
```

### Exemplos de registros inválidos

``` text
50C,30%
30C,110%
abc
```

------------------------------------------------------------------------

## ▶️ Como Executar

1.  Instale o **Python 3** em seu computador;
2.  Baixe ou clone este repositório;
3.  Abra o terminal na pasta do projeto;
4.  Execute:

``` bash
python trabalho.py
```

------------------------------------------------------------------------

## 💻 Exemplo de Saída

``` text
Temperatura: 32.5°C
Fahrenheit: 90.5°F
Umidade: 85%
Sensação: Muito Quente

Resumo do dia:
Registros válidos: 4
Registros inválidos: 2
```

------------------------------------------------------------------------

## 👥 Integrantes

-   **Jéssica Lange Miranda Barbosa**
-   **Sadrack Maia Jesus**

## 🎓 Informações Acadêmicas

**Curso:** Técnico em Inteligência Artificial

**Disciplina:** Programação em Python
