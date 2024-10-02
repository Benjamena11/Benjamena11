# Ejercicios Nivel Básico Python

#EJERCICIO 1 - Edad y Mayoría de Edad

edad = int(input("Escriba su edad:"))

if edad >= 18:

   print("Eres mayor de edad")

else:

   print("Eres menor de edad")

#EJERCICIO 2 - Calificación escolar

calificacion = int(input("Escriba su calificación:"))

if calificacion >=9 and calificacion <= 10:

  print("Sobresaliente")

elif calificacion >= 7 and calificacion < 9:

  print("Aprobado")

elif calificacion < 7 and calificacion >= 0:

  print("Reprobado")

else:

  print("Error")

#EJERCICIO 3 - Nº Negativo, Positivo o Cero

numero = int(input("Escriba un número entero para determinar si es positvo, negativo o cero:"))

if numero > 0:

  print("El número es positivo")

elif numero < 0:

  print("Su número es negativo")

else:

  print("Su número es cero")

#EJERCICIO 4 - Calculadora Simple

num_1 = float(input("Ingrese el primer número:"))

num_2 = float(input("Ingrese el segundo número:"))

operacion = input("Elija un operador para la operación (+, -, *, /):")

if operacion == "+":

  print("El resultado es:",num_1 + num_2)

elif operacion == "-":

  print("El resultado es:", num_1 - num_2)

elif operacion == "*":

  print("El resultado es:", num_1 * num_2)

elif operacion == "/":

  if num_2 != 0:
  
    print("El resultado es:", num_1 / num_2)

  else:
  
    print("Error, no se puede dividir entre cero")

else:

  print("Se equivoco en algún paso, vuelva a intentarlo")

#EJERCICIO 5 - Comparador de Nº

num_1 = float(input("Escriba el primer número:"))

num_2 = float(input("Escriba el segundo número:"))

num_3 = float(input("Escriba el tercer número:"))

if num_1 > num_2 and num_1 > num_3:

  if num_2 > num_3:
  
    print("El primer número es el mayor, y después viene el segundo y tercer número.")
    
  else:
  
    print("El primer número es el mayor, y después viene el tercer y segundo número.")

elif num_2 > num_1 and num_2 > num_3:
  
  if num_1 > num_3:
  
    print("El segundo número es el mayor, y después viene el primer y tercer número.")

  else: 
  
    print("El segundo número es el mayor, y después viene el tercer y primer número.")

elif num_3 > num_1 and num_3 > num_2:

  if num_1 > num_2:
  
    print("El tercer número es el mayor, y después viene el primer y segundo número:")

  else:
  
    print("El tercer número es el mayor, y después viene el segundo y primer número")

#EJERCICIO 6  Comparador Nº simple

num1 = float(input("Ingresa el primer número: "))

num2 = float(input("Ingresa el segundo número: "))

num3 = float(input("Ingresa el tercer número: "))

if num1 >= num2 and num1 >= num3:

    print("El mayor es:", num1)
elif num2 >= num1 and num2 >= num3:

    print("El mayor es:", num2)
else:

    print("El mayor es:", num3)

#EJERCICIO 7 - Validar Contraseña

contraseña_guardada = "Zaki2046"

contraseña_ingresada = input("Ingrese la Contraseña:")

if contraseña_ingresada == contraseña_guardada:

  print("Acceso concedido")

else:

  print("Acceso denegado")

#EJERCICIO 8 - Nº divisible

num_1 = float(input("Escriba el primer número:"))

num_2 = float(input("Escriba el segundo número:"))

if num_2 != 0:

  if num_1 % num_2 == 0:
  
   print("El número", {num_1}, "es divisible por", {num_2})

  else:
  
   print("El número", {num_1}, "no es divisible por", {num_2})

else:

  print("Error: División por cero")

#EJERCICIO 9 - Adivina el Nº

numero_secreto = 7

intento = int(input("Adivina el número secreto (entre 1 y 10): "))

if intento == numero_secreto:

    print("¡Felicidades! Adivinaste el número.")
    
elif intento > numero_secreto:

    print("El número es más pequeño.")
else:

    print("El número es más grande.")

#EJERCICIO 10 - Cálculo Promedio

num_1 = float(input("Calificación 1:"))

num_2 = float(input("Calificación 2:"))

num_3 = float(input("Calificación 3:"))

promedio = (num_1*0.3) + (num_2*0.3) + (num_3*0.4)

if promedio >=3.95 and promedio <=7:

  print(f"El promedio es: {promedio}, Aprobado" )

elif promedio >=1 and promedio <3.95:

  print(f"El promedio es: {promedio}, Reprobado")

else: 

  print("Error, introduzca de nuevo sus calificaciones")

#EJERCICIO 11 - Cálculo Promedio Redondeado

#Definir variables

num_1 = float(input("Calificación 1:"))

num_2 = float(input("Calificación 2:"))

num_3 = float(input("Calificación 3:"))

#Procesamiento

promedio = (num_1*0.3) + (num_2*0.3) + (num_3*0.4)

promedio_redondeado = round(promedio, 1)

if promedio_redondeado >=3.95 and promedio_redondeado <=7:

  print(f"El promedio es: {promedio_redondeado}, Aprobado" )

elif promedio_redondeado >=1 and promedio_redondeado <3.95:

  print(f"El promedio es: {promedio_redondeado}, Reprobado")

else:

  print("Error, introduzca de nuevo sus calificaciones")

#EJERCICIO 12 - Porción e Ingredientes Queque Fiesta

# Definir los ingredientes

ingredientes = {

    'huevos': float(4/10), 
    
    'tazas de harina': float(8/10), 
    
    'taza de leche': float(0.5/10)
}

# Imprimir los ingredientes base para una porción de queque

print("Cuántos ingredientes necesito para hacer una porción de queque:")

for ingrediente, porcion in ingredientes.items():

    print(f"{porcion} {ingrediente}")

# Pedir el número de personas

personas = int(input("¿Cuántas personas asisten a la fiesta?: "))

# Calcular las porciones para la cantidad de personas

fiesta = {ingrediente: porcion * personas for ingrediente, porcion in ingredientes.items()}

# Imprimir los ingredientes necesarios para la cantidad de personas

print(f"Necesitas estos ingredientes para que cada persona tenga una porción de queque:")

for ingrediente, cantidad in fiesta.items():

    print(f"{cantidad} {ingrediente}")

EJERCICIO 13 - Cálculo Rango Etario

#En Chile, si las personas que tienen menos de 18 años, son consideradas menores de edad; aquellas que están en el rango etario de 18 a 35 años se les considera adultos-jóvenes; quienes superan los 35 años, pero aún no alzanzan los 65 años, son consideradas adultos, y los que tiene 65 años o más son consideradas adultos mayores o miembros de la "tercera edad".

#Se solicita que construya un programa en Python que solicite por teclado la edad de una persona e indique su categoría a partir del rango etario dado.

#ENTRADA

#Se solicita la edad de cada persona

edad = int(input("Coloque su edad para indiciar su rango etario: "))

#PROCESAMIENTO

#Se realizan las sentencias condicionales del enunciado

if edad < 18:

    print("Usted es menor de edad")

elif edad >= 18 and edad <= 35:

    print("Usted es un adulto-joven")

elif edad > 35 and edad < 65:

    print("Usted es adulto")

else:

    print("Usted pertenece a la tercera edad")

continuar = input("¿Desea verificar otra edad? (sí/no): ").lower()

if continuar != "sí":

        print("Programa finalizado.")
        
# Rompe el bucle y finaliza el programa
