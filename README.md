# Programa para convertir unidades de longitud entre metros y kilómetros
# Este programa permite al usuario convertir una cantidad de metros a kilómetros o viceversa.

def convertir_metros_a_kilometros(metros):
    """
    Convierte una cantidad de metros a kilómetros.
    
    Parámetros:
    metros (float): La cantidad de metros a convertir.
    
    Retorna:
    float: La cantidad de kilómetros correspondiente.
    """
    return metros / 1000

def convertir_kilometros_a_metros(kilometros):
    """
    Convierte una cantidad de kilómetros a metros.
    
    Parámetros:
    kilometros (float): La cantidad de kilómetros a convertir.
    
    Retorna:
    float: La cantidad de metros correspondiente.
    """
    return kilometros * 1000

def obtener_conversion():
    """
    Solicita al usuario que elija una opción de conversión y luego realiza la conversión
    dependiendo de la opción seleccionada.
    """
    print("Conversor de Longitud")
    print("1. Convertir metros a kilómetros")
    print("2. Convertir kilómetros a metros")
    
    opcion = input("Seleccione una opción (1 o 2): ")
    
    if opcion == "1":
        metros = float(input("Ingrese la cantidad de metros: "))
        kilometros = convertir_metros_a_kilometros(metros)
        print(f"{metros} metros equivalen a {kilometros} kilómetros.")
    elif opcion == "2":
        kilometros = float(input("Ingrese la cantidad de kilómetros: "))
        metros = convertir_kilometros_a_metros(kilometros)
        print(f"{kilometros} kilómetros equivalen a {metros} metros.")
    else:
        print("Opción no válida. Por favor seleccione 1 o 2.")

# Función principal
if __name__ == "__main__":
    obtener_conversion()
