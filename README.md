# Ejercicios_de_Ordenar


Hemos resuelto la tarea "Ejercicios de Ordenar", para la cual hemos creado una carpeta llamada "Clases" en la que se han introducido todas las clases para la correcta realizacion de la tarea. De la misma manera, hemos creado otra carpeta ("Introducir") con archivos para introducir datos (cadenas de texto, numeros y booleanos). Finalmente hemos intoducido los diagramas de flujo y UML correspondientes

## Main

```

if __name__ == "__main__":

    from Clases.Insercion_dicotonomica import Dicotonomia_1, Dicotonomia_2
    print ("Ejercicio 1:")
    print ("Apartado 1")
    tabla = [4,2,6,3,8,7,5,9,1,0]
    print (tabla)
    #Definimos nuestra unica instancia de clase
    resultado = Dicotonomia_1(tabla)
    print ("La tabla ordenada por dicotonomia es: {}".format(resultado.ordenar()))

    print("Apartado 2")
    resultado_2 = Dicotonomia_2(tabla)
    print ("Ordenando a partir de una lista vacia, la lista es:{}".format(resultado_2.ordenar_lista_vacia()))
    print ("\n")

    from Clases.Ordenacion_topologica import Lista
    print ("Ejercicio 2")
    vector = [5,7,3,-4,8,12,9,2,8]
    #Definimos vector como una instancia de la clase Lista
    resultado = Lista(vector)
    #Mostramos el resultado por pantalla
    print ("El resultado tras la ordenacion es el siguiente: {}".format(resultado.ordenacion_burbuja()))
    print ("\n")

    from Clases.Explorar import Segmento
    print ("Ejercicio 3")
    vector = [5,7,3,-4,8,12,9,2,8]
    #Definimos vector como unica instancia de la clase Segmento
    resultado = Segmento(vector)
    #Mostramos por pantalla los segmentos de "vector"
    print ("Los segmentos de {} son: {}".format(vector, resultado.segmentos()))
    print("Tras aplicar la funcion explorar los segmentos quedan de la siguiente manera:")
    #Mostramos por pantalla los segmentos tras aplicar la funcion explorar
    print (resultado.explorar(resultado.segmentos()[0]), " - ", resultado.explorar(resultado.segmentos()[1]))
   
  ยดยดยด
