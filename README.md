print("=-"*13)
print("Conversor de temperatura.")
print("=-"*13)

temp = int(input("""Qual temperatura você tem?
[0] Celsius
[1] Fahrenheit
[2] kelvin 
"""))


if temp == 0:
     C = int(input("""Para qual você quer?
[1] Fahrenheit
[2] Kelvin
"""))
     if C == 1:
          celsius = float(input("Qual é a temperatura? "))
          C_F = (celsius * 1.8) + 32
          print(f"{celsius}° Celsius em Fahrenheit é {C_F}°.")
     if C == 2:
          celsius = float(input("Qual é a temperatura? "))
          C_K = (celsius + 273.15)
          print(f"{celsius}° Celsius em Kelvin é {C_K}°.")

if temp == 1:
     F = int(input("""Para qual você quer?
[0] Celsius
[2] Kelvin
"""))
     if F == 0:
          fahrenheit = float(input("Qual temperatura? "))
          F_C = (fahrenheit - 32) / 1.8
          print(f"{fahrenheit}° Fahrenheit em Celius é {F_C}°.")
     if F == 2:
          fahrenheit = float(input("Qual temperatura? "))
          F_K = (fahrenheit + 459.76) / 1.8
          print(f"{fahrenheit}° Fahrenheit em Kelvin é {F_K}°.")

if temp == 2:
     K = int(input(""""Para qual você quer?
[0] Celsius
[1] Fahrenheit
"""))
     if K == 0:
          kelvin = float(input("Qual temperatura? "))
          K_C = kelvin - 273.15
          print(f"{kelvin}° Kelvin em Celsius é {K_C}°.")
     if K == 1:
          kelvin = float(input("Qual temperatura? "))
          K_F = (kelvin * 1.8) - 459.67
          print(f'{kelvin}° Kelvin em fahrenheit {K_F}°.')
