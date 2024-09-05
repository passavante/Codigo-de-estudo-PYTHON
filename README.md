# Codigo-de-estudo-PYTHON
Código para calculo de horario com entrada 24h e saída 12h.

entrada1 = int(input("DIGITE AS HORAS DA PRIMEIRA ENTRADA: "))
entrada2 = int(input("DIGITE OS MINUTOS DA PRIMEIRA ENTRADA: "))
entrada3 = int(input("DIGITE AS HORAS DA SEGUNDA ENTRADA: "))
entrada4 = int(input("DIGITE OS MINUTOS DA PRIMEIRA ENTRADA: "))
if entrada1>12:
    entrada1 = entrada1-12
if entrada3>12:
    entrada3 = entrada3-12
horas = entrada1 + entrada3
minutos = entrada2 + entrada4
if minutos>=60:
    minutos = minutos - 60
    horas = horas+1
if horas > 12 and minutos<=60:
    horas = horas-12
    minutos = minutos
print(f"Sua saida foi as {horas}:{minutos}")
