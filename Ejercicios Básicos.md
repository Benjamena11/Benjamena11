# Ejercicios Nivel Básico Python

#Ejercicio 1

edad = int(input("Escriba su edad:"))

if edad >= 18:
   print("Eres mayor de edad")

else:
   print("Eres menor de edad")


#Ejercicio 2

calificacion = int(input("Escriba su calificación:"))

if calificacion >=9 and calificacion <= 10:
  print("Sobresaliente")

elif calificacion >= 7 and calificacion < 9:
  print("Aprobado")

elif calificacion < 7 and calificacion >= 0:
  print("Reprobado")

else:
  print("Error")


#Ejercicio 3

numero = int(input("Escriba un número entero para determinar si es positvo, negativo o cero:"))

if numero > 0:
  print("El número es positivo")

elif numero < 0:
  print("Su número es negativo")

else:
  print("Su número es cero")


#Ejercicio 4

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

#Ejercicio 5

