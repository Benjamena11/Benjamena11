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
