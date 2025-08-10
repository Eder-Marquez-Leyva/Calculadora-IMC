# Calculadora-IMC
Fundamentos de Python C35C (Calculadora IMC)

Para realizara esta calculadora IMC se realizo los siguiente 

#solicitamos el  numero de personas a las que se les calculara el IMC

    personas = int(input( "Ingresa el numero total de personas: "))


#Utilizamos el ciclo "while" para hacer hacer las condiciones

    while personas > 0:

#Pedimos los datos al usuario 

    nombre= input("Ingrese su nombre: ")
    apellidopaterno = input("Ingrese su apellido paterno: ")
    apellidomaterno= input("Ingrese su apellido materno: ")
    edad = int(input("Ingrese su edad: "))
    
#uyilizamos un Float por el uso de decimales

    estatura = float(input ("Ingrese su estatura en metros: "))
    peso = float (input("ingrese su peso en kilogramos:"))
    
#colocamos la formula del IMC

    IMC = peso / estatura**2
    print("IMC: " + str(IMC) )
 
#Ejecutamos las validaciones utilizando "if/elif"
    
    if IMC >= 0 and IMC <= 17.99 :
        print ("Peso Bajo")
    elif IMC >= 18.00 and IMC <= 24.99 :
        print ("Peso Normal")
    elif IMC >= 25.00 and IMC <= 29.99:
        print ("Sobrepeso")
    elif IMC >= 30.00 and IMC <= 34.99 :
        print ("Obesidad Leve")
    elif IMC >= 35.00 and IMC <= 39.99:
        print ("Obesdidad Media")
    elif IMC > 40.00 and IMC:
        print ("Obesidad Morbida")
    
#Colocamos la siguiente sentencia para hcer que el ciclo termine
    personas = personas - 1
