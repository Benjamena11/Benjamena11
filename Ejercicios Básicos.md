# Ejercicios Nivel Básico Python

#Operaciones básicas de tipos de datos

nombre = input("Ingrese su nombre:")

edad = input("Ingrese su edad:")

altura = input("Ingrese su altura en metros:")

#1.-Convertir los valores 
edad = int(edad)  
altura = float(altura)  

print(f"Hola {nombre}, tienes {edad} años y mides {altura} metros. Saludos")

print()
print()
print()

#Ejercicios básicos de matemáticas

#1.- Solicita el radio para calcular el área de un círculo
radio = float(input("Ingrese el radio del círculo:"))

#2.- Eacribe fórmula del área de un círculo
area = 3.14* radio**2 

#3.- Imprime el resultado del área
print(f"El área del círculo es: {area}")


