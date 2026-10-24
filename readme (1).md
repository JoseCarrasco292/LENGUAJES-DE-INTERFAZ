# Lenguajes de Interfaz - Repositorio de Prácticas (Irvine32)

## Datos Generales

- **Materia:** Lenguajes de Interfaz
- **Unidad:** Prácticas de Laboratorio (Ensamblador MASM x86 con librería `Irvine32`)
- **Nombre del alumno:** José Mario Carrasco Larios
- **Horario:** 8-9
- **Docente:** Dr. José Luis Medina Jiménez




```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
```

## Índice de Prácticas

| No. | Práctica | Enlace al Código Fuente (`.asm`) | Descripción |
| :--- | :--- | :--- | :--- |
| **1** | Hola Mundo Visual Studio 2022 sin Irvine32 | `Practica0_1_HolaMundoSinIrvine.asm` *(Omitida)* | Programa básico en ensamblador x86 para Visual Studio 2022 sin utilizar la librería Irvine32, empleando llamadas al sistema de Windows API (GetStdHandle, WriteConsoleA y ExitProcess). |
| **2** | Hola Mundo Visual Studio 2022 con Irvine32 | `Practica0_2_HolaMundoConIrvine.asm` *(Omitida)* | Programa básico en ensamblador x86 que despliega un mensaje en consola utilizando el procedimiento WriteString de la librería Irvine32. |
| **3** | Práctica 1. Ciclos numéricos | `Practica1_CiclosNumericos.asm` *(Omitida)* | Implementación de un ciclo numérico controlado por el registro ECX y la instrucción LOOP para desplegar una secuencia de números en pantalla. |
| **4** | Práctica 2. Captura y desplegado de mensaje | [Practica2\_CapturaYDesplegado.asm](https://www.google.com/search?q=./Practica2_CapturaYDesplegado.asm) | Solicita al usuario ingresar una cadena de texto desde la consola utilizando ReadString, la almacena en un búfer en memoria y la despliega nuevamente en pantalla con WriteString. |
| **5** | Práctica 3. Comparación y prueba | [Practica3\_ComparacionYPrueba.asm](https://www.google.com/search?q=./Practica3_ComparacionYPrueba.asm) | Demuestra el uso de la instrucción CMP para comparar dos valores numéricos (25 y 40) y la instrucción TEST para verificar mediante una máscara de bits si un número es par o impar sin alterar el operando destino. |
| **6** | Práctica 4. Saltos | [Practica4\_Saltos.asm](https://www.google.com/search?q=./Practica4_Saltos.asm) | Ejemplifica el control de flujo mediante saltos incondicionales (JMP) para omitir bloques de instrucciones y saltos condicionales (JNZ) para iterar un contador descendente de 5 a 1. |
| **6.1** | Práctica 4.1 Mayor, menor o igual con entrada del usuario | [Practica4\_1\_MayorMenorIgual.asm](https://www.google.com/search?q=./Practica4_1_MayorMenorIgual.asm) | Captura dos números enteros con signo ingresados por el usuario mediante ReadInt, los compara con CMP y utiliza saltos condicionales (JG y JL) para indicar si el primero es mayor, menor o igual al segundo. |
| **7** | Práctica 5. Condicionales | [Practica5\_Condicionales.asm](https://www.google.com/search?q=./Practica5_Condicionales.asm) | Evalúa una calificación numérica (0 a 100) ingresada por el usuario empleando directivas condicionales de alto nivel de MASM (.IF, .ELSEIF y .ELSE) para clasificar el resultado como Excelente, Aprobado o Reprobado. |
| **7.1** | Práctica 5.1 Repetir hasta que el usuario ingrese 0 | [Practica5\_1\_RepetirHastaCero.asm](https://www.google.com/search?q=./Practica5_1_RepetirHastaCero.asm) | Ejecuta un ciclo de captura continua donde pide números enteros al usuario, los suma en un acumulador y muestra cada valor registrado hasta que se ingresa el número 0, momento en que imprime la suma acumulada final. |
| **8** | Práctica 6. Decremento e incremento | [Practica6\_DecrementoEIncremento.asm](https://www.google.com/search?q=./Practica6_DecrementoEIncremento.asm) | Demuestra el funcionamiento de las instrucciones INC y DEC dentro de dos ciclos controlados por LOOP, incrementando una variable desde 10 hasta 15 y posteriormente decrementándola de regreso a 10. |
| **8.1** | Práctica 6.1 Control de ocupación de un estacionamiento | [Practica6\_1\_ControlEstacionamiento.asm](https://www.google.com/search?q=./Practica6_1_ControlEstacionamiento.asm) | Simula un sistema interactivo de control de acceso para un estacionamiento con capacidad máxima de 10 vehículos, permitiendo registrar entradas (INC) y salidas (DEC) mientras valida alertas de cupo lleno o estacionamiento vacío. |
| **9** | Práctica 7. Validación de formato | [Practica7\_ValidacionDeFormato.asm](https://www.google.com/search?q=./Practica7_ValidacionDeFormato.asm) | Valida que una cadena ingresada por el usuario tenga exactamente 4 caracteres de longitud y recorre carácter por carácter verificando que todos se encuentren dentro del rango ASCII numérico ('0' a '9'). |
| **10** | Práctica 8. Operaciones aritméticas | [Practica8\_OperacionesAritmeticas.asm](https://www.google.com/search?q=./Practica8_OperacionesAritmeticas.asm) | Captura dos números enteros con signo y realiza las cuatro operaciones aritméticas básicas: suma (ADD), resta (SUB), multiplicación con signo (IMUL) y división entera con signo (CDQ e IDIV), mostrando tanto el cociente como el residuo. |
| **11** | Práctica 9. Push y Pop | [Practica9\_PushYPop.asm](https://www.google.com/search?q=./Practica9_PushYPop.asm) | Utiliza la pila del sistema (LIFO) mediante las instrucciones PUSH y POP para apilar cada carácter de la cadena 'LENGUAJES DE INTERFAZ' y extraerlos en orden inverso para invertir el texto. |
| **12** | Práctica 10. Cadena con decimal | [Practica10\_CadenaConDecimal.asm](https://www.google.com/search?q=./Practica10_CadenaConDecimal.asm) | Lee un número en formato de cadena ASCII desde el teclado con ReadString, lo convierte a un valor entero binario de 32 bits sin signo mediante ParseDecimal32 y verifica su valor numérico multiplicándolo por dos. |
| **13** | Práctica 11. Operaciones lógicas | [Practica11\_OperacionesLogicas.asm](https://www.google.com/search?q=./Practica11_OperacionesLogicas.asm) | Aplica las operaciones booleanas a nivel de bits (AND, OR, XOR y NOT) sobre dos valores binarios de 8 bits y despliega en consola la representación binaria de cada resultado mediante WriteBinB. |
| **14** | Práctica 12. Desplazamiento y rotación | [Practica12\_DesplazamientoYRotacion.asm](https://www.google.com/search?q=./Practica12_DesplazamientoYRotacion.asm) | Realiza manipulaciones de bits sobre un byte base (10010110b) empleando instrucciones de desplazamiento lógico a la izquierda (SHL) y derecha (SHR), así como rotaciones circulares (ROL y ROR), mostrando cada resultado en binario. |
| **15** | Práctica 13. String hexadecimal | [Practica13\_StringHexadecimal.asm](https://www.google.com/search?q=./Practica13_StringHexadecimal.asm) | Captura un número entero decimal de 32 bits y lo convierte manualmente a una cadena de texto en formato hexadecimal de 8 dígitos extrayendo grupos de 4 bits (nibbles) mediante desplazamientos SHR y una tabla de búsqueda. |
| **16** | Práctica 14. Captura y almacenamiento de dato numérico | [Practica14\_CapturaYAlmacenamientoNumerico.asm](https://www.google.com/search?q=./Practica14_CapturaYAlmacenamientoNumerico.asm) | Solicita al usuario 5 valores numéricos enteros, los almacena secuencialmente en un arreglo de 32 bits utilizando direccionamiento indirecto por registro ([esi]) y luego recorre el arreglo para mostrar todos los elementos guardados. |
| **17** | Práctica 15. Manipulación de archivo | [Practica15\_ManipulacionDeArchivo.asm](https://www.google.com/search?q=./Practica15_ManipulacionDeArchivo.asm) | Captura una línea de texto desde la consola, crea un archivo de salida llamado 'datos_practica15.txt' mediante CreateOutputFile, escribe el contenido capturado usando WriteToFile y cierra el manejador del archivo con CloseFile. |

## Códigos Fuente Comentados (`.asm`)

### 4. Práctica 2. Captura y desplegado de mensaje ([Practica2\_CapturaYDesplegado.asm](https://www.google.com/search?q=./Practica2_CapturaYDesplegado.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 2. Captura y desplegado de mensaje
; Descripción: Solicita al usuario ingresar una cadena de texto desde la consola utilizando ReadString, la almacena en un búfer en memoria y la despliega nuevamente en pantalla con WriteString.

INCLUDE Irvine32.inc              ; Incluye la librería Irvine32 para entrada/salida

.data                             ; Segmento de datos para variables y cadenas
    msgPrompt BYTE "Ingrese un mensaje: ", 0
    msgSalida BYTE "Mensaje capturado: ", 0
    buffer    BYTE 100 DUP(0)     ; Búfer de 100 bytes inicializado en cero para la entrada
    bytesRead DWORD ?             ; Almacena la cantidad de caracteres leídos

.code                             ; Segmento de código
main PROC
    call Clrscr                   ; Limpia la pantalla de la consola

    ; --- Solicitud del mensaje al usuario ---
    mov edx, OFFSET msgPrompt     ; Carga la dirección del mensaje de solicitud en EDX
    call WriteString              ; Imprime el mensaje en consola

    ; --- Captura de la cadena desde el teclado ---
    mov edx, OFFSET buffer        ; EDX apunta al búfer donde se guardará la cadena
    mov ecx, SIZEOF buffer - 1    ; ECX define el máximo de caracteres a leer (dejando espacio para el nulo)
    call ReadString               ; Lee la cadena ingresada; devuelve la longitud en EAX
    mov bytesRead, eax            ; Guarda el número de caracteres leídos

    ; --- Despliegue del mensaje capturado ---
    call Crlf                     ; Inserta un salto de línea
    mov edx, OFFSET msgSalida     ; Carga la dirección de la etiqueta de salida
    call WriteString              ; Muestra "Mensaje capturado: "

    mov edx, OFFSET buffer        ; Apunta EDX al búfer con el texto del usuario
    call WriteString              ; Despliega el mensaje capturado en pantalla
    call Crlf                     ; Salto de línea final

    exit                          ; Termina la ejecución del programa
main ENDP
END main
```

### 5. Práctica 3. Comparación y prueba ([Practica3\_ComparacionYPrueba.asm](https://www.google.com/search?q=./Practica3_ComparacionYPrueba.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 3. Comparación y prueba
; Descripción: Demuestra el uso de la instrucción CMP para comparar dos valores numéricos (25 y 40) y la instrucción TEST para verificar mediante una máscara de bits si un número es par o impar sin alterar el operando destino.

INCLUDE Irvine32.inc              ; Librería de funciones estándar Irvine32

.data                             ; Definición de variables y mensajes
    valA      DWORD 25            ; Primer valor de prueba
    valB      DWORD 40            ; Segundo valor de prueba
    msgCmp    BYTE "Resultado de CMP (25 vs 40): ", 0
    msgMenor  BYTE "El primer valor es menor que el segundo.", 0
    msgMayor  BYTE "El primer valor es mayor o igual al segundo.", 0
    msgTest   BYTE "Resultado de TEST (25 AND 1): ", 0
    msgImpar  BYTE "El numero 25 es impar (Bit 0 encendido).", 0
    msgPar    BYTE "El numero 25 es par (Bit 0 apagado).", 0

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Parte 1: Comparación con la instrucción CMP ---
    mov edx, OFFSET msgCmp        ; Muestra el encabezado de la comparación
    call WriteString

    mov eax, valA                 ; Carga el primer valor (25) en EAX
    cmp eax, valB                 ; Compara EAX con valB (resta implícita: EAX - valB)
    jl EsMenor                    ; Salta a EsMenor si valA < valB (Jump if Less)

    mov edx, OFFSET msgMayor      ; Si no es menor, muestra que es mayor o igual
    call WriteString
    call Crlf
    jmp PruebaBit                 ; Salta a la sección de prueba de bits

EsMenor:
    mov edx, OFFSET msgMenor      ; Imprime mensaje indicando que valA es menor
    call WriteString
    call Crlf

    ; --- Parte 2: Evaluación de bits con la instrucción TEST ---
PruebaBit:
    mov edx, OFFSET msgTest       ; Muestra el encabezado de la prueba lógica
    call WriteString

    mov eax, valA                 ; Carga 25 en EAX
    test eax, 1                   ; Realiza operación AND lógica entre EAX y 1 (verifica el bit menos significativo)
    jnz EsImpar                   ; Si el resultado no es cero (ZF=0), el número es impar

    mov edx, OFFSET msgPar        ; Si ZF=1, el bit 0 está apagado y el número es par
    call WriteString
    call Crlf
    jmp Fin

EsImpar:
    mov edx, OFFSET msgImpar      ; Muestra que el número es impar
    call WriteString
    call Crlf

Fin:
    exit                          ; Finaliza el programa
main ENDP
END main
```

### 6. Práctica 4. Saltos ([Practica4\_Saltos.asm](https://www.google.com/search?q=./Practica4_Saltos.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 4. Saltos
; Descripción: Ejemplifica el control de flujo mediante saltos incondicionales (JMP) para omitir bloques de instrucciones y saltos condicionales (JNZ) para iterar un contador descendente de 5 a 1.

INCLUDE Irvine32.inc              ; Incluye definiciones de Irvine32

.data                             ; Mensajes de seguimiento para los saltos
    msgPaso1  BYTE "Ejecutando Paso 1 (Inicio)...", 0
    msgOmitir BYTE "Este mensaje sera omitido por JMP.", 0
    msgPaso2  BYTE "Ejecutando Paso 2 (Salto incondicional exitoso).", 0
    msgCiclo  BYTE "Iteracion con salto condicional JNZ: ", 0
    msgFin    BYTE "Fin de la demostracion de saltos.", 0

.code
main PROC
    call Clrscr                   ; Limpia la consola

    ; --- Demostración de salto incondicional (JMP) ---
    mov edx, OFFSET msgPaso1      ; Imprime el mensaje inicial
    call WriteString
    call Crlf

    jmp Paso2                     ; Salto incondicional directo hacia la etiqueta Paso2

    ; Este bloque queda inalcanzable gracias al salto JMP anterior
    mov edx, OFFSET msgOmitir
    call WriteString
    call Crlf

Paso2:
    mov edx, OFFSET msgPaso2      ; Confirma que el salto JMP omitió el bloque intermedio
    call WriteString
    call Crlf

    ; --- Demostración de salto condicional (JNZ) en un ciclo ---
    mov ecx, 5                    ; Inicializa el contador en 5 iteraciones

CicloSalto:
    mov edx, OFFSET msgCiclo      ; Imprime etiqueta de iteración
    call WriteString
    mov eax, ecx                  ; Pasa el valor actual del contador a EAX
    call WriteDec                 ; Muestra el número de iteración en decimal
    call Crlf

    dec ecx                       ; Disminuye el contador en 1 (actualiza la bandera Zero Flag)
    jnz CicloSalto                ; Salta a CicloSalto mientras ECX no sea cero (ZF=0)

    mov edx, OFFSET msgFin        ; Mensaje de cierre al terminar las repeticiones
    call WriteString
    call Crlf

    exit
main ENDP
END main
```

### 6.1. Práctica 4.1 Mayor, menor o igual con entrada del usuario ([Practica4\_1\_MayorMenorIgual.asm](https://www.google.com/search?q=./Practica4_1_MayorMenorIgual.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 4.1 Mayor, menor o igual con entrada del usuario
; Descripción: Captura dos números enteros con signo ingresados por el usuario mediante ReadInt, los compara con CMP y utiliza saltos condicionales (JG y JL) para indicar si el primero es mayor, menor o igual al segundo.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Variables de entrada y mensajes de resultado
    msgNum1  BYTE "Ingrese el primer numero entero: ", 0
    msgNum2  BYTE "Ingrese el segundo numero entero: ", 0
    msgMayor BYTE "El primer numero es MAYOR que el segundo.", 0
    msgMenor BYTE "El primer numero es MENOR que el segundo.", 0
    msgIgual BYTE "Ambos numeros son IGUALES.", 0
    num1     SDWORD ?             ; Primer entero de 32 bits con signo
    num2     SDWORD ?             ; Segundo entero de 32 bits con signo

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Captura del primer número ---
    mov edx, OFFSET msgNum1       ; Pide el primer número al usuario
    call WriteString
    call ReadInt                  ; Lee un entero con signo en EAX
    mov num1, eax                 ; Almacena el valor en num1

    ; --- Captura del segundo número ---
    mov edx, OFFSET msgNum2       ; Pide el segundo número al usuario
    call WriteString
    call ReadInt                  ; Lee el segundo entero en EAX
    mov num2, eax                 ; Almacena el valor en num2

    ; --- Comparación y saltos condicionales con signo ---
    mov eax, num1                 ; Mueve num1 a EAX para comparar
    cmp eax, num2                 ; Compara num1 con num2
    jg Mayor                      ; Si num1 > num2 (Jump if Greater), salta a Mayor
    jl Menor                      ; Si num1 < num2 (Jump if Less), salta a Menor

    ; Caso en que ambos números son iguales
    mov edx, OFFSET msgIgual
    call WriteString
    call Crlf
    jmp Salir

Mayor:
    mov edx, OFFSET msgMayor      ; Despliega que el primero es mayor
    call WriteString
    call Crlf
    jmp Salir

Menor:
    mov edx, OFFSET msgMenor      ; Despliega que el primero es menor
    call WriteString
    call Crlf

Salir:
    exit
main ENDP
END main
```

### 7. Práctica 5. Condicionales ([Practica5\_Condicionales.asm](https://www.google.com/search?q=./Practica5_Condicionales.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 5. Condicionales
; Descripción: Evalúa una calificación numérica (0 a 100) ingresada por el usuario empleando directivas condicionales de alto nivel de MASM (.IF, .ELSEIF y .ELSE) para clasificar el resultado como Excelente, Aprobado o Reprobado.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Mensajes y variable para la calificación
    msgPrompt BYTE "Ingrese una calificacion (0-100): ", 0
    msgExc    BYTE "Resultado: Excelente (A)", 0
    msgAprob  BYTE "Resultado: Aprobado (B/C)", 0
    msgReprob BYTE "Resultado: Reprobado (F)", 0
    calif     SDWORD ?            ; Variable con signo para almacenar la calificación

.code
main PROC
    call Clrscr                   ; Limpia la consola

    ; --- Lectura de la calificación ---
    mov edx, OFFSET msgPrompt     ; Solicita la calificación al usuario
    call WriteString
    call ReadInt                  ; Captura el valor entero en EAX
    mov calif, eax                ; Lo guarda en la variable calif

    ; --- Evaluación mediante directivas condicionales de MASM ---
    .IF calif >= 90               ; Verifica si la calificación es mayor o igual a 90
        mov edx, OFFSET msgExc
        call WriteString
    .ELSEIF calif >= 70           ; Verifica si está en rango aprobatorio (70 a 89)
        mov edx, OFFSET msgAprob
        call WriteString
    .ELSE                         ; Cualquier valor menor a 70 es reprobatorio
        mov edx, OFFSET msgReprob
        call WriteString
    .ENDIF

    call Crlf                     ; Salto de línea final
    exit
main ENDP
END main
```

### 7.1. Práctica 5.1 Repetir hasta que el usuario ingrese 0 ([Practica5\_1\_RepetirHastaCero.asm](https://www.google.com/search?q=./Practica5_1_RepetirHastaCero.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 5.1 Repetir hasta que el usuario ingrese 0
; Descripción: Ejecuta un ciclo de captura continua donde pide números enteros al usuario, los suma en un acumulador y muestra cada valor registrado hasta que se ingresa el número 0, momento en que imprime la suma acumulada final.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Mensajes y acumulador de suma
    msgPrompt BYTE "Ingrese un numero (0 para terminar): ", 0
    msgIngres BYTE "Numero registrado: ", 0
    msgSuma   BYTE "Suma acumulada final: ", 0
    acumulado SDWORD 0            ; Acumulador inicializado en 0

.code
main PROC
    call Clrscr                   ; Limpia la consola

    ; --- Ciclo repetitivo controlado por valor centinela (0) ---
CicloCaptura:
    mov edx, OFFSET msgPrompt     ; Pide un número al usuario
    call WriteString
    call ReadInt                  ; Lee el entero en EAX

    cmp eax, 0                    ; Verifica si el número ingresado es 0
    je Terminar                   ; Si es 0 (Jump if Equal), sale del ciclo

    add acumulado, eax            ; Suma el valor ingresado al acumulador

    mov edx, OFFSET msgIngres     ; Confirma el número registrado en pantalla
    call WriteString
    call WriteInt                 ; Imprime el número con signo
    call Crlf
    jmp CicloCaptura              ; Repite el ciclo para pedir otro número

    ; --- Impresión del total acumulado ---
Terminar:
    call Crlf
    mov edx, OFFSET msgSuma       ; Muestra la etiqueta del resultado final
    call WriteString
    mov eax, acumulado            ; Pasa el total acumulado a EAX
    call WriteInt                 ; Despliega la suma final
    call Crlf

    exit
main ENDP
END main
```

### 8. Práctica 6. Decremento e incremento ([Practica6\_DecrementoEIncremento.asm](https://www.google.com/search?q=./Practica6_DecrementoEIncremento.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 6. Decremento e incremento
; Descripción: Demuestra el funcionamiento de las instrucciones INC y DEC dentro de dos ciclos controlados por LOOP, incrementando una variable desde 10 hasta 15 y posteriormente decrementándola de regreso a 10.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Mensajes y variable numérica base
    msgInc BYTE "Incrementando valor con INC: ", 0
    msgDec BYTE "Decrementando valor con DEC: ", 0
    valor  DWORD 10               ; Valor inicial en 10

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Ciclo de incremento con la instrucción INC ---
    mov ecx, 5                    ; Configura 5 repeticiones en ECX
CicloInc:
    inc valor                     ; Incrementa en 1 el contenido de la variable 'valor'
    mov edx, OFFSET msgInc        ; Muestra mensaje de incremento
    call WriteString
    mov eax, valor                ; Carga el valor actual en EAX
    call WriteDec                 ; Imprime el valor en formato decimal sin signo
    call Crlf
    loop CicloInc                 ; Decrementa ECX y repite mientras ECX != 0

    call Crlf                     ; Línea en blanco para separar secciones

    ; --- Ciclo de decremento con la instrucción DEC ---
    mov ecx, 5                    ; Configura 5 repeticiones en ECX
CicloDec:
    dec valor                     ; Decrementa en 1 el contenido de la variable 'valor'
    mov edx, OFFSET msgDec        ; Muestra mensaje de decremento
    call WriteString
    mov eax, valor                ; Carga el valor actual en EAX
    call WriteDec                 ; Imprime el valor actualizado
    call Crlf
    loop CicloDec                 ; Repite hasta completar las 5 iteraciones

    exit
main ENDP
END main
```

### 8.1. Práctica 6.1 Control de ocupación de un estacionamiento ([Practica6\_1\_ControlEstacionamiento.asm](https://www.google.com/search?q=./Practica6_1_ControlEstacionamiento.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 6.1 Control de ocupación de un estacionamiento
; Descripción: Simula un sistema interactivo de control de acceso para un estacionamiento con capacidad máxima de 10 vehículos, permitiendo registrar entradas (INC) y salidas (DEC) mientras valida alertas de cupo lleno o estacionamiento vacío.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Menú, mensajes de estado y contadores del estacionamiento
    msgMenu    BYTE "=== CONTROL DE ESTACIONAMIENTO ===", 13, 10
               BYTE "1. Entrada de vehiculo", 13, 10
               BYTE "2. Salida de vehiculo", 13, 10
               BYTE "3. Salir del sistema", 13, 10
               BYTE "Seleccione una opcion: ", 0
    msgEstado  BYTE "Lugares ocupados: ", 0
    msgDisp    BYTE " | Lugares disponibles: ", 0
    msgLleno   BYTE "Alerta: Estacionamiento lleno. No pueden ingresar mas vehiculos.", 0
    msgVacio   BYTE "Alerta: Estacionamiento vacio. No hay vehiculos para salir.", 0
    capacidad  DWORD 10           ; Cupo máximo del estacionamiento
    ocupados   DWORD 0            ; Contador actual de vehículos dentro

.code
main PROC
    call Clrscr                   ; Limpia la pantalla al iniciar

    ; --- Despliegue del estado actual y menú de opciones ---
MenuLoop:
    call Crlf
    mov edx, OFFSET msgEstado     ; Muestra cantidad de cajones ocupados
    call WriteString
    mov eax, ocupados
    call WriteDec

    mov edx, OFFSET msgDisp       ; Calcula y muestra cajones disponibles (capacidad - ocupados)
    call WriteString
    mov eax, capacidad
    sub eax, ocupados
    call WriteDec
    call Crlf
    call Crlf

    mov edx, OFFSET msgMenu       ; Imprime el menú interactivo
    call WriteString
    call ReadInt                  ; Lee la opción seleccionada por el usuario

    cmp eax, 1                    ; Opción 1: Registrar entrada
    je Entrada
    cmp eax, 2                    ; Opción 2: Registrar salida
    je Salida
    cmp eax, 3                    ; Opción 3: Terminar programa
    je FinPrograma
    jmp MenuLoop                  ; Cualquier otra entrada vuelve a mostrar el menú

    ; --- Lógica de entrada de vehículo ---
Entrada:
    mov eax, ocupados
    cmp eax, capacidad            ; Verifica si ya se alcanzó la capacidad máxima
    jae EstaLleno                 ; Si ocupados >= capacidad, muestra alerta de lleno
    inc ocupados                  ; Incrementa en 1 los lugares ocupados
    jmp MenuLoop

EstaLleno:
    mov edx, OFFSET msgLleno      ; Notifica que no hay lugares disponibles
    call WriteString
    call Crlf
    jmp MenuLoop

    ; --- Lógica de salida de vehículo ---
Salida:
    cmp ocupados, 0               ; Verifica si el estacionamiento está vacío
    je EstaVacio                  ; Si ocupados == 0, impide decrementar bajo cero
    dec ocupados                  ; Decrementa en 1 los lugares ocupados
    jmp MenuLoop

EstaVacio:
    mov edx, OFFSET msgVacio      ; Notifica que no hay autos por salir
    call WriteString
    call Crlf
    jmp MenuLoop

FinPrograma:
    exit
main ENDP
END main
```

### 9. Práctica 7. Validación de formato ([Practica7\_ValidacionDeFormato.asm](https://www.google.com/search?q=./Practica7_ValidacionDeFormato.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 7. Validación de formato
; Descripción: Valida que una cadena ingresada por el usuario tenga exactamente 4 caracteres de longitud y recorre carácter por carácter verificando que todos se encuentren dentro del rango ASCII numérico ('0' a '9').

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Mensajes de validación y búfer de entrada
    msgPrompt   BYTE "Ingrese un codigo numerico de exactamente 4 digitos: ", 0
    msgValido   BYTE "Formato valido: El codigo contiene 4 digitos numericos.", 0
    msgInvalido BYTE "Formato invalido: Debe tener exactamente 4 digitos (0-9).", 0
    buffer      BYTE 20 DUP(0)    ; Espacio para capturar la cadena del usuario

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Captura de la cadena a validar ---
    mov edx, OFFSET msgPrompt
    call WriteString

    mov edx, OFFSET buffer        ; Apunta al búfer de lectura
    mov ecx, SIZEOF buffer - 1
    call ReadString               ; Lee la cadena y devuelve la longitud en EAX

    ; --- Validación 1: Comprobar que la longitud sea exactamente 4 ---
    cmp eax, 4
    jne FormatoInvalido           ; Si no tiene 4 caracteres, el formato es inválido

    ; --- Validación 2: Verificar que cada carácter sea un dígito ('0'-'9') ---
    mov ecx, 4                    ; Contador para revisar los 4 caracteres
    mov esi, OFFSET buffer        ; ESI apunta al primer carácter del búfer

VerificarDigitos:
    mov al, [esi]                 ; Obtiene el carácter actual apuntado por ESI
    cmp al, '0'                   ; Compara con el límite inferior ASCII '0' (48)
    jb FormatoInvalido            ; Si es menor que '0', no es un dígito válido
    cmp al, '9'                   ; Compara con el límite superior ASCII '9' (57)
    ja FormatoInvalido            ; Si es mayor que '9', no es un dígito válido
    inc esi                       ; Avanza al siguiente carácter de la cadena
    loop VerificarDigitos         ; Repite para los 4 caracteres

    ; Si pasa todas las pruebas, el formato es válido
    mov edx, OFFSET msgValido
    call WriteString
    call Crlf
    jmp Salir

FormatoInvalido:
    mov edx, OFFSET msgInvalido   ; Imprime mensaje de error de formato
    call WriteString
    call Crlf

Salir:
    exit
main ENDP
END main
```

### 10. Práctica 8. Operaciones aritméticas ([Practica8\_OperacionesAritmeticas.asm](https://www.google.com/search?q=./Practica8_OperacionesAritmeticas.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 8. Operaciones aritméticas
; Descripción: Captura dos números enteros con signo y realiza las cuatro operaciones aritméticas básicas: suma (ADD), resta (SUB), multiplicación con signo (IMUL) y división entera con signo (CDQ e IDIV), mostrando tanto el cociente como el residuo.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Etiquetas y variables para operandos y resultados
    msgNum1 BYTE "Ingrese el primer numero: ", 0
    msgNum2 BYTE "Ingrese el segundo numero: ", 0
    msgSuma BYTE "Suma (ADD): ", 0
    msgRest BYTE "Resta (SUB): ", 0
    msgMult BYTE "Multiplicacion (IMUL): ", 0
    msgDiv  BYTE "Division (IDIV) Cociente: ", 0
    msgRes  BYTE " | Residuo: ", 0
    num1    SDWORD ?              ; Primer operando con signo
    num2    SDWORD ?              ; Segundo operando con signo
    residuo SDWORD ?              ; Almacena el residuo de la división

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Captura de los dos operandos enteros ---
    mov edx, OFFSET msgNum1
    call WriteString
    call ReadInt
    mov num1, eax

    mov edx, OFFSET msgNum2
    call WriteString
    call ReadInt
    mov num2, eax

    call Crlf

    ; --- Operación 1: Suma (ADD) ---
    mov eax, num1
    add eax, num2                 ; EAX = num1 + num2
    mov edx, OFFSET msgSuma
    call WriteString
    call WriteInt                 ; Muestra el resultado de la suma
    call Crlf

    ; --- Operación 2: Resta (SUB) ---
    mov eax, num1
    sub eax, num2                 ; EAX = num1 - num2
    mov edx, OFFSET msgRest
    call WriteString
    call WriteInt                 ; Muestra el resultado de la resta
    call Crlf

    ; --- Operación 3: Multiplicación con signo (IMUL) ---
    mov eax, num1
    imul num2                     ; EDX:EAX = EAX * num2
    mov edx, OFFSET msgMult
    call WriteString
    call WriteInt                 ; Muestra el producto
    call Crlf

    ; --- Operación 4: División entera con signo (IDIV) ---
    cmp num2, 0                   ; Evita error de división entre cero
    je Fin

    mov eax, num1                 ; Carga el dividendo en EAX
    cdq                           ; Extiende el bit de signo de EAX hacia EDX (forma EDX:EAX)
    idiv num2                     ; Divide EDX:EAX entre num2 -> Cociente en EAX, Residuo en EDX
    mov residuo, edx              ; Guarda el residuo antes de usar EDX para imprimir cadenas

    mov edx, OFFSET msgDiv        ; Muestra el cociente
    call WriteString
    call WriteInt

    mov edx, OFFSET msgRes        ; Muestra el residuo
    call WriteString
    mov eax, residuo
    call WriteInt
    call Crlf

Fin:
    exit
main ENDP
END main
```

### 11. Práctica 9. Push y Pop ([Practica9\_PushYPop.asm](https://www.google.com/search?q=./Practica9_PushYPop.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 9. Push y Pop
; Descripción: Utiliza la pila del sistema (LIFO) mediante las instrucciones PUSH y POP para apilar cada carácter de la cadena 'LENGUAJES DE INTERFAZ' y extraerlos en orden inverso para invertir el texto.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Cadena a invertir y mensajes
    cadena   BYTE "LENGUAJES DE INTERFAZ", 0
    tamano   DWORD ($ - cadena) - 1 ; Calcula automáticamente la longitud sin el carácter nulo
    msgOrig  BYTE "Cadena original:  ", 0
    msgInv   BYTE "Cadena invertida: ", 0

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Muestra la cadena en su orden original ---
    mov edx, OFFSET msgOrig
    call WriteString
    mov edx, OFFSET cadena
    call WriteString
    call Crlf

    ; --- Fase 1: Apilar cada carácter en la pila con PUSH ---
    mov ecx, tamano               ; ECX = número de caracteres de la cadena
    mov esi, 0                    ; Índice inicial en 0

Apilar:
    movzx eax, cadena[esi]        ; Copia el byte actual a EAX extendiendo con ceros
    push eax                      ; Mete el carácter en el tope de la pila (ESP disminuye en 4)
    inc esi                       ; Avanza al siguiente carácter
    loop Apilar                   ; Repite hasta apilar toda la cadena

    ; --- Fase 2: Desapilar caracteres en orden inverso (LIFO) con POP ---
    mov ecx, tamano               ; Reinicia el contador ECX con la longitud de la cadena
    mov esi, 0                    ; Reinicia el índice al principio del arreglo

Desapilar:
    pop eax                       ; Extrae el último carácter apilado hacia EAX (ESP aumenta en 4)
    mov cadena[esi], al           ; Sobrescribe la posición actual con el carácter extraído
    inc esi                       ; Avanza a la siguiente posición
    loop Desapilar                ; Repite hasta vaciar los caracteres de la pila

    ; --- Muestra la cadena ya invertida ---
    mov edx, OFFSET msgInv
    call WriteString
    mov edx, OFFSET cadena
    call WriteString
    call Crlf

    exit
main ENDP
END main
```

### 12. Práctica 10. Cadena con decimal ([Practica10\_CadenaConDecimal.asm](https://www.google.com/search?q=./Practica10_CadenaConDecimal.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 10. Cadena con decimal
; Descripción: Lee un número en formato de cadena ASCII desde el teclado con ReadString, lo convierte a un valor entero binario de 32 bits sin signo mediante ParseDecimal32 y verifica su valor numérico multiplicándolo por dos.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Mensajes, búfer de texto y variable entera resultante
    msgPrompt BYTE "Ingrese una cadena numerica decimal: ", 0
    msgResult BYTE "Valor entero convertido (ParseDecimal32): ", 0
    msgDoble  BYTE "Valor multiplicado por 2 para verificar: ", 0
    buffer    BYTE 32 DUP(0)      ; Búfer para almacenar los dígitos como texto ASCII
    numero    DWORD ?             ; Variable donde se guardará el entero ya convertido

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Captura del número como cadena de caracteres ---
    mov edx, OFFSET msgPrompt
    call WriteString

    mov edx, OFFSET buffer        ; EDX apunta al búfer de entrada
    mov ecx, SIZEOF buffer - 1
    call ReadString               ; Lee el texto; EAX contiene la longitud leída

    ; --- Conversión de cadena ASCII a entero de 32 bits ---
    mov edx, OFFSET buffer        ; EDX apunta al inicio de la cadena numérica
    mov ecx, eax                  ; ECX indica cuántos caracteres componen la cadena
    call ParseDecimal32           ; Convierte el texto ASCII a entero binario en EAX
    mov numero, eax               ; Guarda el número convertido en memoria

    ; --- Despliegue del valor entero convertido ---
    mov edx, OFFSET msgResult
    call WriteString
    mov eax, numero
    call WriteDec                 ; Imprime el valor numérico
    call Crlf

    ; --- Operación aritmética de prueba sobre el número convertido ---
    mov edx, OFFSET msgDoble
    call WriteString
    mov eax, numero
    shl eax, 1                    ; Multiplica por 2 desplazando un bit a la izquierda
    call WriteDec                 ; Muestra el doble del número para comprobar la conversión
    call Crlf

    exit
main ENDP
END main
```

### 13. Práctica 11. Operaciones lógicas ([Practica11\_OperacionesLogicas.asm](https://www.google.com/search?q=./Practica11_OperacionesLogicas.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 11. Operaciones lógicas
; Descripción: Aplica las operaciones booleanas a nivel de bits (AND, OR, XOR y NOT) sobre dos valores binarios de 8 bits y despliega en consola la representación binaria de cada resultado mediante WriteBinB.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Valores binarios de prueba y etiquetas descriptivas
    valA    DWORD 10101100b       ; Primer operando binario (ACh)
    valB    DWORD 00001111b       ; Segundo operando binario / máscara (0Fh)
    msgValA BYTE "Valor A (binario): ", 0
    msgValB BYTE "Valor B (binario): ", 0
    msgAnd  BYTE "Resultado AND:     ", 0
    msgOr   BYTE "Resultado OR:      ", 0
    msgXor  BYTE "Resultado XOR:     ", 0
    msgNot  BYTE "Resultado NOT A:   ", 0

.code
main PROC
    call Clrscr                   ; Limpia la consola

    ; --- Muestra los valores originales en formato binario de 1 byte ---
    mov edx, OFFSET msgValA
    call WriteString
    mov eax, valA
    mov ebx, TYPE BYTE            ; Especifica impresión de 1 byte (8 bits) para WriteBinB
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgValB
    call WriteString
    mov eax, valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf
    call Crlf

    ; --- Operación lógica AND (conserva bits donde ambos son 1) ---
    mov edx, OFFSET msgAnd
    call WriteString
    mov eax, valA
    and eax, valB                 ; EAX = valA AND valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    ; --- Operación lógica OR (enciende bits donde al menos uno es 1) ---
    mov edx, OFFSET msgOr
    call WriteString
    mov eax, valA
    or eax, valB                  ; EAX = valA OR valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    ; --- Operación lógica XOR (enciende bits donde los operandos son distintos) ---
    mov edx, OFFSET msgXor
    call WriteString
    mov eax, valA
    xor eax, valB                 ; EAX = valA XOR valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    ; --- Operación lógica NOT (invierte todos los bits del operando) ---
    mov edx, OFFSET msgNot
    call WriteString
    mov eax, valA
    not al                        ; Invierte los 8 bits inferiores en AL (complemento a 1)
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    exit
main ENDP
END main
```

### 14. Práctica 12. Desplazamiento y rotación ([Practica12\_DesplazamientoYRotacion.asm](https://www.google.com/search?q=./Practica12_DesplazamientoYRotacion.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 12. Desplazamiento y rotación
; Descripción: Realiza manipulaciones de bits sobre un byte base (10010110b) empleando instrucciones de desplazamiento lógico a la izquierda (SHL) y derecha (SHR), así como rotaciones circulares (ROL y ROR), mostrando cada resultado en binario.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Byte de prueba y etiquetas para cada operación de bits
    valorBase BYTE 10010110b      ; Patrón de 8 bits inicial
    msgBase   BYTE "Valor original:         ", 0
    msgSHL    BYTE "Desplazamiento SHL 1:   ", 0
    msgSHR    BYTE "Desplazamiento SHR 1:   ", 0
    msgROL    BYTE "Rotacion ROL 2:         ", 0
    msgROR    BYTE "Rotacion ROR 2:         ", 0

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Muestra el valor binario original ---
    mov edx, OFFSET msgBase
    call WriteString
    movzx eax, valorBase          ; Carga el byte en EAX limpiando la parte alta
    mov ebx, TYPE BYTE            ; Formato de salida de 8 bits
    call WriteBinB
    call Crlf

    ; --- Desplazamiento lógico a la izquierda (SHL) ---
    mov edx, OFFSET msgSHL
    call WriteString
    movzx eax, valorBase
    shl al, 1                     ; Desplaza los bits 1 posición a la izquierda (inserta 0 a la derecha)
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    ; --- Desplazamiento lógico a la derecha (SHR) ---
    mov edx, OFFSET msgSHR
    call WriteString
    movzx eax, valorBase
    shr al, 1                     ; Desplaza los bits 1 posición a la derecha (inserta 0 a la izquierda)
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    ; --- Rotación circular a la izquierda (ROL) ---
    mov edx, OFFSET msgROL
    call WriteString
    movzx eax, valorBase
    rol al, 2                     ; Rota 2 bits a la izquierda (los que salen por la izq. entran por la der.)
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    ; --- Rotación circular a la derecha (ROR) ---
    mov edx, OFFSET msgROR
    call WriteString
    movzx eax, valorBase
    ror al, 2                     ; Rota 2 bits a la derecha (los que salen por la der. entran por la izq.)
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    exit
main ENDP
END main
```

### 15. Práctica 13. String hexadecimal ([Practica13\_StringHexadecimal.asm](https://www.google.com/search?q=./Practica13_StringHexadecimal.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 13. String hexadecimal
; Descripción: Captura un número entero decimal de 32 bits y lo convierte manualmente a una cadena de texto en formato hexadecimal de 8 dígitos extrayendo grupos de 4 bits (nibbles) mediante desplazamientos SHR y una tabla de búsqueda.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Tabla de conversión hexadecimal y búfer de salida
    msgPrompt BYTE "Ingrese un numero entero decimal: ", 0
    msgHexOut BYTE "Cadena hexadecimal generada: ", 0
    tablaHex  BYTE "0123456789ABCDEF" ; Tabla de traducción de nibble (0-15) a carácter ASCII
    strHex    BYTE 8 DUP('0'), "h", 0 ; Cadena de 8 dígitos hexadecimales terminada en 'h'
    valor     DWORD ?

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Lectura del número decimal sin signo ---
    mov edx, OFFSET msgPrompt
    call WriteString
    call ReadDec                  ; Lee el entero en EAX
    mov valor, eax

    ; --- Conversión de cada nibble (4 bits) a carácter hexadecimal ---
    mov ecx, 8                    ; Un DWORD de 32 bits contiene 8 dígitos hexadecimales
    mov edi, OFFSET strHex + 7    ; Apunta al último dígito de la cadena (escritura de derecha a izquierda)
    mov ebx, OFFSET tablaHex      ; Dirección base de la tabla de caracteres hexadecimales

ConvertirHex:
    mov edx, eax                  ; Copia el valor actual a EDX
    and edx, 0Fh                  ; Aísla los 4 bits menos significativos (nibble inferior)
    mov dl, [ebx + edx]           ; Obtiene el carácter ASCII equivalente desde tablaHex
    mov [edi], dl                 ; Almacena el carácter en la posición actual de strHex
    shr eax, 4                    ; Desplaza EAX 4 bits a la derecha para procesar el siguiente nibble
    dec edi                       ; Retrocede una posición en la cadena destino
    loop ConvertirHex             ; Repite para los 8 dígitos

    ; --- Despliegue de la cadena hexadecimal resultante ---
    mov edx, OFFSET msgHexOut
    call WriteString
    mov edx, OFFSET strHex        ; Imprime la cadena formateada (ej. 000000FFh)
    call WriteString
    call Crlf

    exit
main ENDP
END main
```

### 16. Práctica 14. Captura y almacenamiento de dato numérico ([Practica14\_CapturaYAlmacenamientoNumerico.asm](https://www.google.com/search?q=./Practica14_CapturaYAlmacenamientoNumerico.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 14. Captura y almacenamiento de dato numérico
; Descripción: Solicita al usuario 5 valores numéricos enteros, los almacena secuencialmente en un arreglo de 32 bits utilizando direccionamiento indirecto por registro ([esi]) y luego recorre el arreglo para mostrar todos los elementos guardados.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Declaración del arreglo y mensajes
    MAX_ELEM   = 5                ; Constante que define el tamaño del arreglo
    arreglo    SDWORD MAX_ELEM DUP(?) ; Arreglo de 5 enteros con signo sin inicializar
    msgPrompt  BYTE "Ingrese un dato numerico para almacenar: ", 0
    msgMostrar BYTE "Datos numericos almacenados en el arreglo:", 13, 10, 0
    msgSep     BYTE "  ", 0

.code
main PROC
    call Clrscr                   ; Limpia la pantalla

    ; --- Fase 1: Captura y almacenamiento en el arreglo ---
    mov ecx, MAX_ELEM             ; Inicializa el contador del ciclo en 5 elementos
    mov esi, OFFSET arreglo       ; ESI apunta al primer elemento del arreglo

CicloCaptura:
    mov edx, OFFSET msgPrompt     ; Solicita el dato numérico
    call WriteString
    call ReadInt                  ; Lee el entero desde teclado hacia EAX
    mov [esi], eax                ; Almacena el número en la posición de memoria apuntada por ESI
    add esi, TYPE SDWORD          ; Avanza el puntero ESI 4 bytes hacia el siguiente elemento
    loop CicloCaptura             ; Repite hasta llenar los 5 espacios

    ; --- Fase 2: Recorrido e impresión de los datos almacenados ---
    call Crlf
    mov edx, OFFSET msgMostrar
    call WriteString

    mov ecx, MAX_ELEM             ; Reinicia el contador en 5
    mov esi, OFFSET arreglo       ; Vuelve a apuntar ESI al inicio del arreglo

CicloDespliegue:
    mov eax, [esi]                ; Recupera el entero almacenado en la dirección actual de ESI
    call WriteInt                 ; Muestra el número en consola
    mov edx, OFFSET msgSep        ; Imprime espacio separador
    call WriteString
    add esi, TYPE SDWORD          ; Avanza al siguiente elemento (4 bytes)
    loop CicloDespliegue          ; Repite para mostrar todos los elementos

    call Crlf
    exit
main ENDP
END main
```

### 17. Práctica 15. Manipulación de archivo ([Practica15\_ManipulacionDeArchivo.asm](https://www.google.com/search?q=./Practica15_ManipulacionDeArchivo.asm))

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 15. Manipulación de archivo
; Descripción: Captura una línea de texto desde la consola, crea un archivo de salida llamado 'datos_practica15.txt' mediante CreateOutputFile, escribe el contenido capturado usando WriteToFile y cierra el manejador del archivo con CloseFile.

INCLUDE Irvine32.inc              ; Librería Irvine32

.data                             ; Nombre de archivo, búfer de texto y variables de control
    nombreArchivo BYTE "datos_practica15.txt", 0
    msgPrompt     BYTE "Ingrese el texto a guardar en el archivo: ", 0
    msgExito      BYTE "Archivo creado y escrito correctamente.", 0
    msgError      BYTE "Error al crear el archivo.", 0
    buffer        BYTE 256 DUP(0) ; Búfer para el texto que se escribirá en disco
    longitud      DWORD ?         ; Cantidad de caracteres capturados
    manejador     HANDLE ?        ; Handle (identificador) del archivo abierto
    bytesEscritos DWORD ?         ; Número de bytes efectivamente escritos

.code
main PROC
    call Clrscr                   ; Limpia la consola

    ; --- Captura del texto que se guardará en el archivo ---
    mov edx, OFFSET msgPrompt
    call WriteString

    mov edx, OFFSET buffer        ; EDX apunta al búfer de entrada
    mov ecx, SIZEOF buffer - 1
    call ReadString               ; Captura el texto y devuelve su longitud en EAX
    mov longitud, eax             ; Guarda la longitud exacta del texto

    ; --- Creación y apertura del archivo de salida ---
    mov edx, OFFSET nombreArchivo ; EDX contiene el nombre del archivo a crear
    call CreateOutputFile         ; Crea el archivo y devuelve el handle en EAX
    mov manejador, eax            ; Guarda el manejador del archivo

    cmp eax, INVALID_HANDLE_VALUE ; Verifica si ocurrió un error al crear el archivo
    je ErrorArchivo               ; Si el handle es inválido, salta al manejo de error

    ; --- Escritura del búfer dentro del archivo ---
    mov eax, manejador            ; EAX = handle del archivo abierto
    mov edx, OFFSET buffer        ; EDX = dirección de los datos a escribir
    mov ecx, longitud             ; ECX = cantidad de bytes a escribir
    call WriteToFile              ; Escribe los datos en el archivo
    mov bytesEscritos, eax        ; Guarda el total de bytes escritos

    ; --- Cierre del archivo y confirmación ---
    mov eax, manejador            ; Pasa el handle del archivo a EAX
    call CloseFile                ; Cierra el archivo para asegurar la escritura en disco

    mov edx, OFFSET msgExito      ; Muestra confirmación de éxito
    call WriteString
    call Crlf
    jmp Salir

ErrorArchivo:
    mov edx, OFFSET msgError      ; Informa en caso de fallo al crear el archivo
    call WriteString
    call Crlf

Salir:
    exit
main ENDP
END main
```
