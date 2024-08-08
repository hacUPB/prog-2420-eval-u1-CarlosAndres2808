# Problemas
## Problema 1:
1-Entrada de datos

    -Lista de calificaciones de Ana 

2-Cálcular el promedio

    -Sumar las calificaciones
    -Contar el número total de calificaciones 
    -Dividir el total con el número de calificaciones que se contaron

3-Evalaur 

    -Comparar el promedio calculado con el que se necesita (3.0)
    -Si el promedio es igual o mayor a (3.0) Ana aprobó
    -Si el promedio es menor a (3.0) Ana reprobó

4-Salida de datos

    -Mostrar el promedio de calificaciones
    -Imprimir 

### Pseudocódigo

Inicio
    Definir la lista de calificaciones
    calificaciones = [lista de calificaciones]
    Iniciar variables
    suma = 0
    cantidad = (calificaciones) // Número de calificaciones
    Calcular la suma de todas las calificaciones
    PARA cada calificacion en calificaciones HACER
        suma = suma + calificacion
    FIN PARA
    Calcular el promedio
        promedio = suma / cantidad
    Verificar si el promedio es suficiente para aprobar
    SI promedio >= 3.0 ENTONCES
        IMPRIMIR "Ana ha aprobado con un promedio de " + promedio
    SINO
        IMPRIMIR "Ana no ha aprobado. Su promedio es " + promedio
    FIN SI
FIN

## Problema 2:
1-Definir los registros:

    -Hacer dos listas, una para las velocidades y otra para los tiempos.

2-Iniciar las variables:

    -Crear una variable para acumular la distancia recorrida.

3-Calcular la distancia:

    -Registrar las velocidades y el tiempo
    -Calcular la distancia recorrida en cada intervalo de tiempo con la siguiente formula:
    D=V*T
    -Sumar la distancia recorrida en cada intervalo a la distancia total.

4-Mostrar el resultado:

    -Imprimir la distancia total que se recorrió.

### Pseudocódigo

Inicio
    Definir los registros de velocidad y tiempo
    velocidades = [lista de velocidades]
    tiempos = [lista de tiempos]
    Iniciar la variable para la distancia total
    distancia_total = 0
    Calcular la distancia recorrida en cada intervalo
    PARA i DESDE 0 HASTA(velocidades) - 1 HACER
        velocidad = velocidades[i]
        tiempo = tiempos[i]
        distancia_intervalo = velocidad * tiempo
        distancia_total = distancia_total + distancia_intervalo
    FIN PARA
    Mostrar el resultado
    IMPRIMIR "La distancia total recorrida es " + distancia_total
FIN

## Problema 3: 

1-Entrada: 

    -Fecha de nacimiento (día/mes/año)
    -Fecha actual (día/mes/año)

2-Cálculos iniciales:

    -Calcular la diferencia en años entre la fecha actual y la fecha de nacimiento.
    -Organizar la diferencia en años en función de si la persona ya cumplio años en el año presente.

3-Cálculo de los meses y días:

    -Organizar los dias teniendo en cuenta si el cumpleaños de la persona ya pasó en el año actual.
    -Utilizar las fechas de nacimiento y las fechas actuales para calcular el número exacto de meses y días.

4-Determinar el día de cumpleaños:

    -Verificar que la fecha actual coincida con la fecha de nacimiento y así se sabe el cumpleaños de la persona.

5-Salida:

    -Edad en años,meses y días.
    -Indicar si ya cumplio años o cuando es su cumpleaños.

### Pseudocódigo

Inicio
    -Entradas
        Leer dia_nacimiento
        Leer mes_nacimiento
        Leer año_nacimiento
        Leer dia_actual
        Leer mes_actual
        Leer año_actual

    -Calcular la edad en años
        edad_años = año_actual - año_nacimiento

    -Ajustar la edad si el cumpleaños no ha pasado este año 
        Si (mes_actual < mes_nacimiento) o (mes_actual = mes_nacimiento y dia_actual < dia_nacimiento) Entonces
        edad_años ← edad_años - 1
    FinSi

    -Calcular la diferencia en meses y días
        meses = mes_actual - mes_nacimiento
        dias = dia_actual - dia_nacimiento
    Sino
        meses = mes_actual - mes_nacimiento - 1
        dias = (días en el mes anterior a la fecha_actual) - (días desde el inicio del mes hasta la fecha_nacimiento)
    FinSi

    -Ajustar los días si hay un desajuste en el cálculo
    Si dias < 0 Entonces
        meses = meses - 1
        dias = (días en el mes actual) + dias
    FinSi

    -Determinar si hoy es el cumpleaños
        es_cumpleanos - (dia_actual = dia_nacimiento) y (mes_actual = mes_nacimiento)

    -Determinar si ya ha cumplido años este año
        ya_cumplido = (mes_actual > mes_nacimiento) o (mes_actual = mes_nacimiento y dia_actual >= dia_nacimiento)

    -Imprimir resultados
         "Edad: "  años + meses, + dias "
         "¿Es hoy su cumpleaños? " + (es_cumpleaños ? "Sí" : "No")
        "¿Ya ha cumplido años este año? " + (ya_cumplido ? "Sí" : "No")
Fin



