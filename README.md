# ¿Largo? Un poquito no más 
He aquí el repo del  RETO#4 
En cada uno de los archivos está cada uno de los puntos del reto #4
## 1.Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.
Primero tuve que identificar los números pertenecientes al codigo ASCII (sí, cuando lo escribí, en mi cabeza sonó aski) de cada una de las vocales en minúscua, para la a:97, para la e:101, para la i:105, para la o:111 y para la u:117. Con ayuda de una estructura if-elif dar una condición con cada uno de estos números.
```pseudocode
print("Ingrese un numero entero")
numerito = float(input("Su número: "))
if numerito == 97:
    print("El número que ingresó corresponde a la vocal 'a' en el código ASCII")
elif numerito == 101:
    print("El número que ingresó corresponde a la vocal 'e' en el código ASCII")
elif numerito == 105:
    print("El número que ingresó corresponde a la vocal 'i' en el código ASCII")
elif numerito == 111:
    print("El número que ingresó corresponde a la vocal 'o' en el código ASCII")
elif numerito == 117:
    print("El número que ingresó corresponde a la vocal 'u' en el código ASCII")
else:
    print("El número que ingresó no corresponde a alguna vocal minúscula en código ASCII")
```
## 2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no
Con cadena de longitud 1 entendí que era una cadena de un solo carácter. Con la función ord (que da el codigo ASCII de un carácter) definí una variable y despues con una operación modulo igualada a 0 cree una condición en una estructura if-else.
```pseudocode
la_cadenita = (input("Ingrese una letra: "))
codigo = ord(la_cadenita)
if codigo % 2 == 0:
    print("El código ASCII de primera letra de la cadena es par")
else:
    print("El codigo ASCII de la primera letra de la cadena es impar")
```
## 3.Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no
Parae ste punto con ayuda de una estructura if-else cree la condición cuando el caracter es igual a algún digito (0,1,2,3,4,5,6,7,8,9)
```pseudocode
el_susodicho = (input("Ingrese un carácter: "))
if el_susodicho == "0" or el_susodicho == "1" or el_susodicho == "2" or el_susodicho == "3" or el_susodicho == "4" or el_susodicho == "5" or el_susodicho == "6" or el_susodicho == "7" or el_susodicho == "8" or el_susodicho == "9":
    print("El carácter ingresado corresponde a un dígito")
else:
    print("El carácter ingresado no corresponde a un dígito")
```
