import UIKit
//ejercicio 1

for i in 1...10 {
    print (i)
}

var numero = 1
while numero <= 10{
    print(numero)
    numero += 1
}

var contador = 1
repeat {
    print(contador)
    contador += 1
} while numero <= 10
            
// ejercicio 2 imprime los SOLO los numeros pares del 1 al 20 utilizando el bucle for.

for pares in 1...20{
    if pares % 2==0{
        print(pares)
    }
}
//ejercicio 3 Utilizando el bucle for agrega los valores [ 2 , 4 , 6 , 8 , 10] al arreglo

var arreglo : [Int] = []

for nummer in 2...10{
    if nummer % 2==0{
        arreglo.append(nummer)
    }
}
print(arreglo)
//ejercico 4 Impime una cuenta regresiva del 10 al 1 usando while

var das_nummer=10

while das_nummer >= 1{
    print(das_nummer)
    das_nummer -= 1
}

//ejercico 5 Crea una funcion que no reciba parametros llamada nombreCompleto que imprima tu nombre

func nombreCompleto(){
    let nombre = "obed"
    print(nombre)
}
nombreCompleto()

//ejercicio 6 Crea una funcion que reciba como parametros tu nombre y apellido e imprima "Hola soy nombre apellido

func nombreparametro(nombre: String,apellido: String){
    print("hola soy \(nombre), \(apellido)")
}
nombreparametro(nombre: "obed", apellido: "rodriguez")

//ejercicio 7
func areatriangulo(base: Double,altura: Double){
   base*altura
}
areatriangulo(base: 5.2, altura: 2.5)
//ejercicio 8
