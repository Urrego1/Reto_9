# Reto_9

1. De los retos anteriores selecione 3 funciones y escribalas en forma de lambdas.

a) Diseñe una función que calcule la cantidad de carne de aves en kilos si se tienen N gallinas, M gallos y K pollitos cada uno pesando 6 kilos, 7 kilos y 1 kilo respectivamente.

```python

N=int(input("Cúal es el numero total de gallinas? "))
M=int(input("Cúal es el numero total de gallos? "))
K=int(input("Cúal es el numero total de pollitos? "))

masa=lambda N,M,K:(N*6)+(K*1)+(M*7)

total=masa(N,M,K)
print("La cantidad total de carne de aves es "+str(total)+" kilogramos")

```

b) Haga un programa que utilice una función para calcular el valor de un préstamo C usando interés compuesto del i por n meses.
  ```python
    if __name__ == "__main__":

    C = float(input("¿Cúal es el total de prestamo?: "))
    I = float(input("¿Cúanto es el porcentaje del interes?: "))
    N = float(input("¿Por cuantos meses es el plazo?: "))

    interes = lambda C,I,N : C * ((1+(I/100))**N) #Función anonima para calcular el interes compuesto.
    valor_int_comp = interes(C,I,N) #Da valor a la variable "valor_int_comp" utilzando la función anonima.

    print("En este caso, el total del interes compuesto es de " + str(valor_int_comp)) 
```


 c) El número de contagiados de Covid-19 en el país de NuncaLandia se duplica cada día. Hacer un programa que diga el número total de personas que se han contagiado cuando pasen D días a partir de hoy, si el número de contagiados actuales es C.
 
```python
C=int(input("Número de contagiados de Covid-19 en el dia 0 "))
D=int(input("Número de días"))
n=1
while n<=D:
  funcion=lambda C:C*2
  pacientes=funcion(C)
  C=C*2
  n+=1
print("El número de pacientes contagiados en Nuncalandia es de "+str(C))

```




2. De los retos anteriores selecione 3 funciones y escribalas con argumentos no definidos (*args).

a) El número de contagiados de Covid-19 en el país de NuncaLandia se duplica cada día. Hacer un programa que diga el número total de personas que se han contagiado cuando pasen D días a partir de hoy, si el número de contagiados actuales es C.

```python

def duplicar(*args)-> int:
  dup : int = 0
  for num in args:
    dup=num*2
  return dup
n=1
if __name__ == "__main__":
  C=int(input("Número de contagiados de Covid-19 en el dia 0 "))
  D=int(input("Número de días"))
  while n<=D:
    C=duplicar(C)
    n+=1
print("El número de pacientes contagiados en Nuncalandia es de "+str(C))

```

b) Diseñe una función que calcule la cantidad de carne de aves en kilos si se tienen N gallinas, M gallos y K pollitos cada uno pesando 6 kilos, 7 kilos y 1 kilo respectivamente

```python

def masa_total(*args)->int:
  suma:int=0
  for num in args:
    suma+=num
  return suma
if __name__ == "__main__":
  N=int(input("Cúal es el numero total de gallinas? "))
  M=int(input("Cúal es el numero total de gallos? "))
  K=int(input("Cúal es el numero total de pollitos? "))
  X=N*6
  Y=M*7
  Z=K*1
  print("La cantidad total de carne de aves es "+str(masa_total(X,Y,Z))+" kilogramos")
```

c) Cuadrado de un número


```python

def list(*args)-> int:
  cuadrado : int = 0
  for num in args:
    cuadrado=num**2
  return cuadrado
if __name__ == "__main__":
    square = int(input("Ingrese un numero de su preferencia: "))
    print("El cuadrado del numero ingresado es " + str(list(square)))

```





3. Escriba una función recursiva para calcular la operación de la potencia.

```python

#Se hace la función recursiva
def potencia(B, P):
    if P == 0:
        return 1
    else: 
        return B ** P
if __name__ == "__main__":
  B=int(input("Ingresa una base "))
  P=int(input("ingresa una potencia "))
  operacion = potencia(B, P)
  print("el numero" str(B)+ " elevado a " +str(P)+" es "+str(operacion))

```


4. Utilice la siguiente plantilla de code para contar el tiempo:

```python

import time

start_time = time.time()
# instrucciones sobre las cuales se quiere medir tiempo de ejecución
end_time = time.time()

timer = end_time - start_time
print(timer)

```

5. Crear cuenta en stackoverflow y adjuntar imagen en el repo
 ![image](https://github.com/Urrego1/Reto_9/assets/159048641/e7192bde-ad1f-4bea-9313-0cd5d9ba3e4a)



6. ir a linkedin y crear perfil

   link https://www.linkedin.com/in/alejandro-urrego-valencia-760338216/
