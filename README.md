# Projeto-Python-Tec.-IA-
Conversor e Validador de Dados Climáticos de Manaus

# Lista de registros
dados = [
    "32.5C,85%",
    "28C,70%",
    "40C,95%",
    "15C,50%",
    "50C,30%",   # temperatura inválida
    "30C,110%",  # umidade inválida
    "abc"         # dado corrompido
]

# Converter Celsius para Fahrenheit
def celsius_para_fahrenheit(c):
    return (c * 9/5) + 32

# Classificar sensação térmica
def sensacao(temp, umidade):
    if temp >= 35 and umidade >= 80:
        return "Muito Quente"
    elif temp >= 30:
        return "Quente"
    elif temp >= 20:
        return "Agradável"
    else:
        return "Frio"

validos = 0
invalidos = 0

print("=== RELATÓRIO CLIMÁTICO ===\n")

for registro in dados:
    try:
        partes = registro.split(",")

        temperatura = float(partes[0].replace("C", ""))
        umidade = int(partes[1].replace("%", ""))

        # Validação
        if not (0 <= temperatura <= 45):
            raise ValueError("Temperatura fora da faixa")

        if not (0 <= umidade <= 100):
            raise ValueError("Umidade fora da faixa")

        fahrenheit = celsius_para_fahrenheit(temperatura)
        classificacao = sensacao(temperatura, umidade)

        print(f"Registro: {registro}")
        print(f"Temperatura: {temperatura:.1f}°C")
        print(f"Fahrenheit: {fahrenheit:.1f}°F")
        print(f"Umidade: {umidade}%")
        print(f"Sensação: {classificacao}")
        print("-" * 30)

        validos += 1

    except:
        print(f"Registro inválido: {registro}")
        print("-" * 30)
        invalidos += 1

print("\n=== RESUMO DO DIA ===")
print(f"Registros válidos: {validos}")
print(f"Registros inválidos: {invalidos}")
