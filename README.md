# Sistema-Cine-Matriz
Sistema de administración de asientos para cine basado en matrices


 1.  Identificación del Problema
 
 Descripción: Un cine desea automatizar y digitalizar por completo el proceso de administración de asientos para evitar los errores humanos comunes en las reservaciones manuales (como la             sobreventa, duplicidad de lugares o la pérdida de control de la sala).  
 Objetivo: Desarrollar un sistema de software que permita visualizar el estado de la sala y gestionar el ciclo de vida de los asientos de forma eficiente.  
 
 2. Entradas, Procesos y Salidas (EPS)
   
-Entradas (Lo que el usuario ingresa al sistema)

La opción del menú principal elegida (ej. reservar, liberar, consultar, etc.).

Las coordenadas del asiento deseadas (número de fila y número de columna).

Procesos (Lo que el sistema calcula o valida internamente):
Inicialización: Crear y rellenar la matriz de la sala con un valor que represente un estado libre (por ejemplo, con el carácter 'L').

Validación de límites: Comprobar que la fila y la columna ingresadas por el usuario existan físicamente dentro de las dimensiones de la matriz.

Verificación de disponibilidad: Revisar si el asiento seleccionado está libre antes de permitir una reservación (para evitar encimar lugares).

Actualización: Cambiar el estado del asiento en la matriz (de libre a ocupado, o viceversa).

Cálculos matemáticos: Recorrer con ciclos la matriz para sumar cuántos asientos están ocupados, cuántos están disponibles y calcular el porcentaje total de ocupación.   

-Salidas (Lo que el sistema le muestra al usuario):
La representación gráfica y ordenada de la matriz de la sala en la pantalla. 
Mensajes de confirmación o de error (ej. "Asiento reservado con éxito" o "El asiento ya está ocupado").Reportes con las estadísticas de ocupación de la sala.

 4. Justificación de la Estructura de DatosEstructura elegida: Una matriz bidimensional (arreglo de dos dimensiones) de tamaño fijo.Justificación: Es la estructura ideal porque simula de manera exacta y natural la distribución física de una sala de cine real (organizada en filas y columnas de butacas). Esto permite un acceso directo, rápido y lógico a cualquier asiento utilizando sus coordenadas exactas de fila y columna
 5. Alcance y LimitacionesAlcance: Control de una sala de cine mediante consola o interfaz básica, gestión completa de reservas, liberaciones, consultas de disponibilidad y estadísticas de ocupación.   Limitaciones: El almacenamiento de los datos es temporal en la memoria RAM durante la ejecución del programa (no incluye base de datos externa permanente).
