# Reto 10: Arreglos
## 1. Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.
```python
#Desarrollar un algoritmo que calcule el promedio de un arreglo de reales

n = int(input("Ingrese la cantidad de elementos que desea que tenga el arreglo ")) #se ingresa por teclado la cantidad que el usuario quiera
reales = [] #se crea una lista vacía

for i in range (n): #para cada número dentro del rango de n:
  a = float(input("Ingrese el elemento #" +str(i+1)+ " real para el arreglo "))  #preguntar qué elementos irán dentro del arreglo
  reales.append(a) #agregar dichos elementos en la lista creada anteriormente

suma_reales = 0 # se parte desde 0 para ser iterada la variable dentro del ciclo for

for i in range(n):
  suma_reales +=reales[i] #se suman todos los elementos que pertenecen a 'reales' 

promedio:float = suma_reales /len(reales) #se calcula el promedio con la suma anterior y con la cantidad de elementos en el arreglo

print(reales)
print("El promedio numérico del arreglo es " +str(promedio))
```
## 2. Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.
```python
#Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.

n = int(input("Ingrese la cantidad de elementos que desea que tengan los arreglos ")) #se ingresa por teclado la cantidad que el usuario quiera

arreglo1= [] #se crea una lista vacía
for i in range(n): #para cada número dentro del rango de n:
  a = float(input("Ingrese el elemento entero #" +str(i+1)+ " para el primer arreglo ")) #preguntar qué elementos irán dentro del primer arreglo
  arreglo1.append(a) #agregar los elementos al primer arreglo

arreglo2=[] #lista vacía
for i in range(n):
  b = float(input("Ingrese el elemento entero #" +str(i+1)+ "  para el segundo arreglo ")) #preguntar los elementos que irán en el segundo arreglo 
  arreglo2.append(b) #agregar elementos al segundo arreglo

producto_punto = 0 #variable a ser iterada dentro del ciclo for, se inicia en 0 para que no afecte el resultado
for i in range(n):
    producto_punto += arreglo1[i]*arreglo2[i] #se va recorriendo cada elemento y este a su vez se multiplica por otro elemento en el otro arreglo con la misma posición 

print(arreglo1) 
print(arreglo2)
print("El producto punto entre los dos arreglos es " +str(producto_punto))
```
## 3. Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.
```python
# Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.
n = int(input("Ingrese la cantidad de elementos que desea que tenga el arreglo ")) #se ingresa por teclado la cantidad que el usuario quiera
arreglo = [] #se crea una lista vacía

for i in range (n): #para cada número dentro del rango de n:
  a = float(input("Ingrese el elemento #" +str(i+1)+ " para el arreglo, algunos de estos elementos deben ser igual a 0 "))  #preguntar qué elementos irán dentro del arreglo
  arreglo.append(a) #agregar dichos elementos en la lista creada anteriormente

numeros = [] #se crean dos listas vacías
ceros = []

for i in range(len(arreglo)): #evaluar cada elemento si es igual a 0 o no
  if arreglo[i] != 0:
    numeros.append(arreglo[i]) #agregar al arreglo de numeros diferentes de 0
  else:
    ceros.append(arreglo[i]) #agegar al arreglo de numeros iguales a 0

arreglo = numeros + ceros #concatenar con los dos arreglos auxiliares
print(arreglo)
```
