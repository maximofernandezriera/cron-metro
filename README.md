# Ejercicio del cronómetro digital

    // ##################################################################################################################
    // Realizar un procedimiento que simule un cronómetro digital, indicando  por pantalla las horas, minutos y segundos.
    // ##################################################################################################################
    
    // Análisis del ejercicio:
    
    // Necesito realizar 3 bucles anidados: el más interno es que me permite recorrer
    // los segundos, el intermedio me permite recorrer los minutos y el más externo
    // recorre las horas. 
    // Datos de entrada: Nada
    // Información de salida por pantalla: La hora (hora, minutos y segundos)
    // Variables: hora,minuto,segundo (entero)
    
    // NOTA1: Existe una función propia del sistema operativo (no la tenemos que hacer nosotros) 
    // que limpia la pantalla, es decir que resetea los valores del cronómetro (00:00:00), llamada Limpiar Pantalla.
    // NOTA2: Existe una función propia del sistema operativo (no la tenemos que hacer nosotros) 
    // que pausa el proceso 1 segundo llamado Esperar 1 Segundo.
    // ################################################################################

    Proceso Cronometro
      Definir hora,minuto,Segundo Como Entero
      Para hora<-0 Hasta 23 Hacer // Bucle horas
        Para minuto<-0 Hasta 59 Hacer // Bucle minutos
          Para Segundo<-0 Hasta 59 Hacer // Bucle segundos
            Borrar Pantalla
            // escribe hora:minutos:segundos (actualizandose a medida que va pasando cada segundo)
            Escribir hora,':',minuto,':',Segundo
            Esperar 1 Segundo
          FinPara
        FinPara
      FinPara
    FinProceso

