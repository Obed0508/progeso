import Foundation

var ciclo : String = ""

var numero1 : Double = 0
var numero2 : Double = 0

func suma(n1: Double,n2: Double){
    let resultado = n1 + n2
    print("El resultado de la suma es: \(resultado)")
}

func resta(n1: Double,n2: Double){
    let resultado = n1 - n2
    print("El resultado de la resta es: \(resultado)")
}

func multiplicacion(n1: Double,n2: Double){
    let resultado = n1 * n2
    print("El resultado de la multiplicacion es: \(resultado)")
}

func divison(n1: Double,n2: Double){
    var resultado : Double = 0
    if n2 == 0 {
        print("la dfivision no se puede realizar")
    }else {
        resultado = n1 / n2
        print("El resultado de la division es: \(resultado)")
    }
    
    
    
    while ciclo != "salir" {
        print("Ingresa un numero: ")
        numero1 = Double(readLine() ?? "0") ?? 0
        print("ingrese un numero: ")
        numero2 = Double(readLine() ?? "0") ?? 0
        print("Ingrese la opcion deseada")
        print("suma")
        print("resta")
        print("multiplicacion")
        print("division")
        ciclo = readLine() ?? "salir"
        switch ciclo {
        case "suma" :
            suma(n1: numero1, n2: numero2)
        case "resta":
            resta(n1: numero1, n2: numero2)
        case "multiplicacion":
            multiplicacion(n1: numero1, n2: numero2)
        case "division":
            divison(n1: numero1, n2: numero2)
        case "salir":
            break
        default :
            print("algo salio mal")
            
        }
    }
    
}
