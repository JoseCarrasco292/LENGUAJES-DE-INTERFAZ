# Prácticas de Lenguajes de Interfaz (Irvine32)

## Datos Generales

- **Materia:** Lenguajes de Interfaz
- **Alumno:** José Mario Carrasco Larios
- **Horario:** 8-9
- **Docente:** Dr. José Luis Medina Jiménez
- **Librería:** `Irvine32.inc` (MASM x86 - Visual Studio 2022)

## Formato de Encabezado Estándar

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
```

## Índice General de Prácticas

| No. | Práctica | Archivo | Descripción |
| :--- | :--- | :--- | :--- |
| **1** | Hola Mundo Visual Studio 2022 sin Irvine32 | `Practica0_1_HolaMundoSinIrvine.asm` | Programa básico en ensamblador x86 para Visual Studio 2022 sin utilizar la librería Irvine32, empleando llamadas al sistema de Windows API (GetStdHandle, WriteConsoleA y ExitProcess). |
| **2** | Hola Mundo Visual Studio 2022 con Irvine32 | `Practica0_2_HolaMundoConIrvine.asm` | Programa básico en ensamblador x86 que despliega un mensaje en consola utilizando el procedimiento WriteString de la librería Irvine32. |
| **3** | Práctica 1. Ciclos numéricos | `Practica1_CiclosNumericos.asm` | Implementación de un ciclo numérico controlado por el registro ECX y la instrucción LOOP para desplegar una secuencia de números en pantalla. |
| **4** | Práctica 2. Captura y desplegado de mensaje | `Practica2_CapturaYDesplegado.asm` | Solicita al usuario ingresar una cadena de texto desde la consola utilizando ReadString, la almacena en un búfer en memoria y la despliega nuevamente en pantalla con WriteString. |
| **5** | Práctica 3. Comparación y prueba | `Practica3_ComparacionYPrueba.asm` | Demuestra el uso de la instrucción CMP para comparar dos valores numéricos (25 y 40) y la instrucción TEST para verificar mediante una máscara de bits si un número es par o impar sin alterar el operando destino. |
| **6** | Práctica 4. Saltos | `Practica4_Saltos.asm` | Ejemplifica el control de flujo mediante saltos incondicionales (JMP) para omitir bloques de instrucciones y saltos condicionales (JNZ) para iterar un contador descendente de 5 a 1. |
| **6.1** | Práctica 4.1 Mayor, menor o igual con entrada del usuario | `Practica4_1_MayorMenorIgual.asm` | Captura dos números enteros con signo ingresados por el usuario mediante ReadInt, los compara con CMP y utiliza saltos condicionales (JG y JL) para indicar si el primero es mayor, menor o igual al segundo. |
| **7** | Práctica 5. Condicionales | `Practica5_Condicionales.asm` | Evalúa una calificación numérica (0 a 100) ingresada por el usuario empleando directivas condicionales de alto nivel de MASM (.IF, .ELSEIF y .ELSE) para clasificar el resultado como Excelente, Aprobado o Reprobado. |
| **7.1** | Práctica 5.1 Repetir hasta que el usuario ingrese 0 | `Practica5_1_RepetirHastaCero.asm` | Ejecuta un ciclo de captura continua donde pide números enteros al usuario, los suma en un acumulador y muestra cada valor registrado hasta que se ingresa el número 0, momento en que imprime la suma acumulada final. |
| **8** | Práctica 6. Decremento e incremento | `Practica6_DecrementoEIncremento.asm` | Demuestra el funcionamiento de las instrucciones INC y DEC dentro de dos ciclos controlados por LOOP, incrementando una variable desde 10 hasta 15 y posteriormente decrementándola de regreso a 10. |
| **8.1** | Práctica 6.1 Control de ocupación de un estacionamiento | `Practica6_1_ControlEstacionamiento.asm` | Simula un sistema interactivo de control de acceso para un estacionamiento con capacidad máxima de 10 vehículos, permitiendo registrar entradas (INC) y salidas (DEC) mientras valida alertas de cupo lleno o estacionamiento vacío. |
| **9** | Práctica 7. Validación de formato | `Practica7_ValidacionDeFormato.asm` | Valida que una cadena ingresada por el usuario tenga exactamente 4 caracteres de longitud y recorre carácter por carácter verificando que todos se encuentren dentro del rango ASCII numérico ('0' a '9'). |
| **10** | Práctica 8. Operaciones aritméticas | `Practica8_OperacionesAritmeticas.asm` | Captura dos números enteros con signo y realiza las cuatro operaciones aritméticas básicas: suma (ADD), resta (SUB), multiplicación con signo (IMUL) y división entera con signo (CDQ e IDIV), mostrando tanto el cociente como el residuo. |
| **11** | Práctica 9. Push y Pop | `Practica9_PushYPop.asm` | Utiliza la pila del sistema (LIFO) mediante las instrucciones PUSH y POP para apilar cada carácter de la cadena 'LENGUAJES DE INTERFAZ' y extraerlos en orden inverso para invertir el texto. |
| **12** | Práctica 10. Cadena con decimal | `Practica10_CadenaConDecimal.asm` | Lee un número en formato de cadena ASCII desde el teclado con ReadString, lo convierte a un valor entero binario de 32 bits sin signo mediante ParseDecimal32 y verifica su valor numérico multiplicándolo por dos. |
| **13** | Práctica 11. Operaciones lógicas | `Practica11_OperacionesLogicas.asm` | Aplica las operaciones booleanas a nivel de bits (AND, OR, XOR y NOT) sobre dos valores binarios de 8 bits y despliega en consola la representación binaria de cada resultado mediante WriteBinB. |
| **14** | Práctica 12. Desplazamiento y rotación | `Practica12_DesplazamientoYRotacion.asm` | Realiza manipulaciones de bits sobre un byte base (10010110b) empleando instrucciones de desplazamiento lógico a la izquierda (SHL) y derecha (SHR), así como rotaciones circulares (ROL y ROR), mostrando cada resultado en binario. |
| **15** | Práctica 13. String hexadecimal | `Practica13_StringHexadecimal.asm` | Captura un número entero decimal de 32 bits y lo convierte manualmente a una cadena de texto en formato hexadecimal de 8 dígitos extrayendo grupos de 4 bits (nibbles) mediante desplazamientos SHR y una tabla de búsqueda. |
| **16** | Práctica 14. Captura y almacenamiento de dato numérico | `Practica14_CapturaYAlmacenamientoNumerico.asm` | Solicita al usuario 5 valores numéricos enteros, los almacena secuencialmente en un arreglo de 32 bits utilizando direccionamiento indirecto por registro ([esi]) y luego recorre el arreglo para mostrar todos los elementos guardados. |
| **17** | Práctica 15. Manipulación de archivo | `Practica15_ManipulacionDeArchivo.asm` | Captura una línea de texto desde la consola, crea un archivo de salida llamado 'datos_practica15.txt' mediante CreateOutputFile, escribe el contenido capturado usando WriteToFile y cierra el manejador del archivo con CloseFile. |

## Detalle de Códigos y Encabezados (Prácticas 2 a 15)

### 4. Práctica 2. Captura y desplegado de mensaje (`Practica2_CapturaYDesplegado.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 2. Captura y desplegado de mensaje
; Descripción: Solicita al usuario ingresar una cadena de texto desde la consola utilizando ReadString, la almacena en un búfer en memoria y la despliega nuevamente en pantalla con WriteString.

INCLUDE Irvine32.inc

.data
    msgPrompt BYTE "Ingrese un mensaje: ", 0
    msgSalida BYTE "Mensaje capturado: ", 0
    buffer    BYTE 100 DUP(0)
    bytesRead DWORD ?

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgPrompt
    call WriteString

    mov edx, OFFSET buffer
    mov ecx, SIZEOF buffer - 1
    call ReadString
    mov bytesRead, eax

    call Crlf
    mov edx, OFFSET msgSalida
    call WriteString

    mov edx, OFFSET buffer
    call WriteString
    call Crlf

    exit
main ENDP
END main
```

### 5. Práctica 3. Comparación y prueba (`Practica3_ComparacionYPrueba.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 3. Comparación y prueba
; Descripción: Demuestra el uso de la instrucción CMP para comparar dos valores numéricos (25 y 40) y la instrucción TEST para verificar mediante una máscara de bits si un número es par o impar sin alterar el operando destino.

INCLUDE Irvine32.inc

.data
    valA      DWORD 25
    valB      DWORD 40
    msgCmp    BYTE "Resultado de CMP (25 vs 40): ", 0
    msgMenor  BYTE "El primer valor es menor que el segundo.", 0
    msgMayor  BYTE "El primer valor es mayor o igual al segundo.", 0
    msgTest   BYTE "Resultado de TEST (25 AND 1): ", 0
    msgImpar  BYTE "El numero 25 es impar (Bit 0 encendido).", 0
    msgPar    BYTE "El numero 25 es par (Bit 0 apagado).", 0

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgCmp
    call WriteString

    mov eax, valA
    cmp eax, valB
    jl EsMenor

    mov edx, OFFSET msgMayor
    call WriteString
    call Crlf
    jmp PruebaBit

EsMenor:
    mov edx, OFFSET msgMenor
    call WriteString
    call Crlf

PruebaBit:
    mov edx, OFFSET msgTest
    call WriteString

    mov eax, valA
    test eax, 1
    jnz EsImpar

    mov edx, OFFSET msgPar
    call WriteString
    call Crlf
    jmp Fin

EsImpar:
    mov edx, OFFSET msgImpar
    call WriteString
    call Crlf

Fin:
    exit
main ENDP
END main
```

### 6. Práctica 4. Saltos (`Practica4_Saltos.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 4. Saltos
; Descripción: Ejemplifica el control de flujo mediante saltos incondicionales (JMP) para omitir bloques de instrucciones y saltos condicionales (JNZ) para iterar un contador descendente de 5 a 1.

INCLUDE Irvine32.inc

.data
    msgPaso1  BYTE "Ejecutando Paso 1 (Inicio)...", 0
    msgOmitir BYTE "Este mensaje sera omitido por JMP.", 0
    msgPaso2  BYTE "Ejecutando Paso 2 (Salto incondicional exitoso).", 0
    msgCiclo  BYTE "Iteracion con salto condicional JNZ: ", 0
    msgFin    BYTE "Fin de la demostracion de saltos.", 0

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgPaso1
    call WriteString
    call Crlf

    jmp Paso2

    mov edx, OFFSET msgOmitir
    call WriteString
    call Crlf

Paso2:
    mov edx, OFFSET msgPaso2
    call WriteString
    call Crlf

    mov ecx, 5

CicloSalto:
    mov edx, OFFSET msgCiclo
    call WriteString
    mov eax, ecx
    call WriteDec
    call Crlf

    dec ecx
    jnz CicloSalto

    mov edx, OFFSET msgFin
    call WriteString
    call Crlf

    exit
main ENDP
END main
```

### 6.1. Práctica 4.1 Mayor, menor o igual con entrada del usuario (`Practica4_1_MayorMenorIgual.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 4.1 Mayor, menor o igual con entrada del usuario
; Descripción: Captura dos números enteros con signo ingresados por el usuario mediante ReadInt, los compara con CMP y utiliza saltos condicionales (JG y JL) para indicar si el primero es mayor, menor o igual al segundo.

INCLUDE Irvine32.inc

.data
    msgNum1  BYTE "Ingrese el primer numero entero: ", 0
    msgNum2  BYTE "Ingrese el segundo numero entero: ", 0
    msgMayor BYTE "El primer numero es MAYOR que el segundo.", 0
    msgMenor BYTE "El primer numero es MENOR que el segundo.", 0
    msgIgual BYTE "Ambos numeros son IGUALES.", 0
    num1     SDWORD ?
    num2     SDWORD ?

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgNum1
    call WriteString
    call ReadInt
    mov num1, eax

    mov edx, OFFSET msgNum2
    call WriteString
    call ReadInt
    mov num2, eax

    mov eax, num1
    cmp eax, num2
    jg Mayor
    jl Menor

    mov edx, OFFSET msgIgual
    call WriteString
    call Crlf
    jmp Salir

Mayor:
    mov edx, OFFSET msgMayor
    call WriteString
    call Crlf
    jmp Salir

Menor:
    mov edx, OFFSET msgMenor
    call WriteString
    call Crlf

Salir:
    exit
main ENDP
END main
```

### 7. Práctica 5. Condicionales (`Practica5_Condicionales.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 5. Condicionales
; Descripción: Evalúa una calificación numérica (0 a 100) ingresada por el usuario empleando directivas condicionales de alto nivel de MASM (.IF, .ELSEIF y .ELSE) para clasificar el resultado como Excelente, Aprobado o Reprobado.

INCLUDE Irvine32.inc

.data
    msgPrompt BYTE "Ingrese una calificacion (0-100): ", 0
    msgExc    BYTE "Resultado: Excelente (A)", 0
    msgAprob  BYTE "Resultado: Aprobado (B/C)", 0
    msgReprob BYTE "Resultado: Reprobado (F)", 0
    calif     SDWORD ?

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgPrompt
    call WriteString
    call ReadInt
    mov calif, eax

    .IF calif >= 90
        mov edx, OFFSET msgExc
        call WriteString
    .ELSEIF calif >= 70
        mov edx, OFFSET msgAprob
        call WriteString
    .ELSE
        mov edx, OFFSET msgReprob
        call WriteString
    .ENDIF

    call Crlf
    exit
main ENDP
END main
```

### 7.1. Práctica 5.1 Repetir hasta que el usuario ingrese 0 (`Practica5_1_RepetirHastaCero.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 5.1 Repetir hasta que el usuario ingrese 0
; Descripción: Ejecuta un ciclo de captura continua donde pide números enteros al usuario, los suma en un acumulador y muestra cada valor registrado hasta que se ingresa el número 0, momento en que imprime la suma acumulada final.

INCLUDE Irvine32.inc

.data
    msgPrompt BYTE "Ingrese un numero (0 para terminar): ", 0
    msgIngres BYTE "Numero registrado: ", 0
    msgSuma   BYTE "Suma acumulada final: ", 0
    acumulado SDWORD 0

.code
main PROC
    call Clrscr

CicloCaptura:
    mov edx, OFFSET msgPrompt
    call WriteString
    call ReadInt

    cmp eax, 0
    je Terminar

    add acumulado, eax

    mov edx, OFFSET msgIngres
    call WriteString
    call WriteInt
    call Crlf
    jmp CicloCaptura

Terminar:
    call Crlf
    mov edx, OFFSET msgSuma
    call WriteString
    mov eax, acumulado
    call WriteInt
    call Crlf

    exit
main ENDP
END main
```

### 8. Práctica 6. Decremento e incremento (`Practica6_DecrementoEIncremento.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 6. Decremento e incremento
; Descripción: Demuestra el funcionamiento de las instrucciones INC y DEC dentro de dos ciclos controlados por LOOP, incrementando una variable desde 10 hasta 15 y posteriormente decrementándola de regreso a 10.

INCLUDE Irvine32.inc

.data
    msgInc BYTE "Incrementando valor con INC: ", 0
    msgDec BYTE "Decrementando valor con DEC: ", 0
    valor  DWORD 10

.code
main PROC
    call Clrscr

    mov ecx, 5
CicloInc:
    inc valor
    mov edx, OFFSET msgInc
    call WriteString
    mov eax, valor
    call WriteDec
    call Crlf
    loop CicloInc

    call Crlf

    mov ecx, 5
CicloDec:
    dec valor
    mov edx, OFFSET msgDec
    call WriteString
    mov eax, valor
    call WriteDec
    call Crlf
    loop CicloDec

    exit
main ENDP
END main
```

### 8.1. Práctica 6.1 Control de ocupación de un estacionamiento (`Practica6_1_ControlEstacionamiento.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 6.1 Control de ocupación de un estacionamiento
; Descripción: Simula un sistema interactivo de control de acceso para un estacionamiento con capacidad máxima de 10 vehículos, permitiendo registrar entradas (INC) y salidas (DEC) mientras valida alertas de cupo lleno o estacionamiento vacío.

INCLUDE Irvine32.inc

.data
    msgMenu    BYTE "=== CONTROL DE ESTACIONAMIENTO ===", 13, 10
               BYTE "1. Entrada de vehiculo", 13, 10
               BYTE "2. Salida de vehiculo", 13, 10
               BYTE "3. Salir del sistema", 13, 10
               BYTE "Seleccione una opcion: ", 0
    msgEstado  BYTE "Lugares ocupados: ", 0
    msgDisp    BYTE " | Lugares disponibles: ", 0
    msgLleno   BYTE "Alerta: Estacionamiento lleno. No pueden ingresar mas vehiculos.", 0
    msgVacio   BYTE "Alerta: Estacionamiento vacio. No hay vehiculos para salir.", 0
    capacidad  DWORD 10
    ocupados   DWORD 0

.code
main PROC
    call Clrscr

MenuLoop:
    call Crlf
    mov edx, OFFSET msgEstado
    call WriteString
    mov eax, ocupados
    call WriteDec

    mov edx, OFFSET msgDisp
    call WriteString
    mov eax, capacidad
    sub eax, ocupados
    call WriteDec
    call Crlf
    call Crlf

    mov edx, OFFSET msgMenu
    call WriteString
    call ReadInt

    cmp eax, 1
    je Entrada
    cmp eax, 2
    je Salida
    cmp eax, 3
    je FinPrograma
    jmp MenuLoop

Entrada:
    mov eax, ocupados
    cmp eax, capacidad
    jae EstaLleno
    inc ocupados
    jmp MenuLoop

EstaLleno:
    mov edx, OFFSET msgLleno
    call WriteString
    call Crlf
    jmp MenuLoop

Salida:
    cmp ocupados, 0
    je EstaVacio
    dec ocupados
    jmp MenuLoop

EstaVacio:
    mov edx, OFFSET msgVacio
    call WriteString
    call Crlf
    jmp MenuLoop

FinPrograma:
    exit
main ENDP
END main
```

### 9. Práctica 7. Validación de formato (`Practica7_ValidacionDeFormato.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 7. Validación de formato
; Descripción: Valida que una cadena ingresada por el usuario tenga exactamente 4 caracteres de longitud y recorre carácter por carácter verificando que todos se encuentren dentro del rango ASCII numérico ('0' a '9').

INCLUDE Irvine32.inc

.data
    msgPrompt   BYTE "Ingrese un codigo numerico de exactamente 4 digitos: ", 0
    msgValido   BYTE "Formato valido: El codigo contiene 4 digitos numericos.", 0
    msgInvalido BYTE "Formato invalido: Debe tener exactamente 4 digitos (0-9).", 0
    buffer      BYTE 20 DUP(0)

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgPrompt
    call WriteString

    mov edx, OFFSET buffer
    mov ecx, SIZEOF buffer - 1
    call ReadString

    cmp eax, 4
    jne FormatoInvalido

    mov ecx, 4
    mov esi, OFFSET buffer

VerificarDigitos:
    mov al, [esi]
    cmp al, '0'
    jb FormatoInvalido
    cmp al, '9'
    ja FormatoInvalido
    inc esi
    loop VerificarDigitos

    mov edx, OFFSET msgValido
    call WriteString
    call Crlf
    jmp Salir

FormatoInvalido:
    mov edx, OFFSET msgInvalido
    call WriteString
    call Crlf

Salir:
    exit
main ENDP
END main
```

### 10. Práctica 8. Operaciones aritméticas (`Practica8_OperacionesAritmeticas.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 8. Operaciones aritméticas
; Descripción: Captura dos números enteros con signo y realiza las cuatro operaciones aritméticas básicas: suma (ADD), resta (SUB), multiplicación con signo (IMUL) y división entera con signo (CDQ e IDIV), mostrando tanto el cociente como el residuo.

INCLUDE Irvine32.inc

.data
    msgNum1 BYTE "Ingrese el primer numero: ", 0
    msgNum2 BYTE "Ingrese el segundo numero: ", 0
    msgSuma BYTE "Suma (ADD): ", 0
    msgRest BYTE "Resta (SUB): ", 0
    msgMult BYTE "Multiplicacion (IMUL): ", 0
    msgDiv  BYTE "Division (IDIV) Cociente: ", 0
    msgRes  BYTE " | Residuo: ", 0
    num1    SDWORD ?
    num2    SDWORD ?
    residuo SDWORD ?

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgNum1
    call WriteString
    call ReadInt
    mov num1, eax

    mov edx, OFFSET msgNum2
    call WriteString
    call ReadInt
    mov num2, eax

    call Crlf

    mov eax, num1
    add eax, num2
    mov edx, OFFSET msgSuma
    call WriteString
    call WriteInt
    call Crlf

    mov eax, num1
    sub eax, num2
    mov edx, OFFSET msgRest
    call WriteString
    call WriteInt
    call Crlf

    mov eax, num1
    imul num2
    mov edx, OFFSET msgMult
    call WriteString
    call WriteInt
    call Crlf

    cmp num2, 0
    je Fin

    mov eax, num1
    cdq
    idiv num2
    mov residuo, edx

    mov edx, OFFSET msgDiv
    call WriteString
    call WriteInt

    mov edx, OFFSET msgRes
    call WriteString
    mov eax, residuo
    call WriteInt
    call Crlf

Fin:
    exit
main ENDP
END main
```

### 11. Práctica 9. Push y Pop (`Practica9_PushYPop.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 9. Push y Pop
; Descripción: Utiliza la pila del sistema (LIFO) mediante las instrucciones PUSH y POP para apilar cada carácter de la cadena 'LENGUAJES DE INTERFAZ' y extraerlos en orden inverso para invertir el texto.

INCLUDE Irvine32.inc

.data
    cadena   BYTE "LENGUAJES DE INTERFAZ", 0
    tamano   DWORD ($ - cadena) - 1
    msgOrig  BYTE "Cadena original:  ", 0
    msgInv   BYTE "Cadena invertida: ", 0

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgOrig
    call WriteString
    mov edx, OFFSET cadena
    call WriteString
    call Crlf

    mov ecx, tamano
    mov esi, 0

Apilar:
    movzx eax, cadena[esi]
    push eax
    inc esi
    loop Apilar

    mov ecx, tamano
    mov esi, 0

Desapilar:
    pop eax
    mov cadena[esi], al
    inc esi
    loop Desapilar

    mov edx, OFFSET msgInv
    call WriteString
    mov edx, OFFSET cadena
    call WriteString
    call Crlf

    exit
main ENDP
END main
```

### 12. Práctica 10. Cadena con decimal (`Practica10_CadenaConDecimal.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 10. Cadena con decimal
; Descripción: Lee un número en formato de cadena ASCII desde el teclado con ReadString, lo convierte a un valor entero binario de 32 bits sin signo mediante ParseDecimal32 y verifica su valor numérico multiplicándolo por dos.

INCLUDE Irvine32.inc

.data
    msgPrompt BYTE "Ingrese una cadena numerica decimal: ", 0
    msgResult BYTE "Valor entero convertido (ParseDecimal32): ", 0
    msgDoble  BYTE "Valor multiplicado por 2 para verificar: ", 0
    buffer    BYTE 32 DUP(0)
    numero    DWORD ?

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgPrompt
    call WriteString

    mov edx, OFFSET buffer
    mov ecx, SIZEOF buffer - 1
    call ReadString

    mov edx, OFFSET buffer
    mov ecx, eax
    call ParseDecimal32
    mov numero, eax

    mov edx, OFFSET msgResult
    call WriteString
    mov eax, numero
    call WriteDec
    call Crlf

    mov edx, OFFSET msgDoble
    call WriteString
    mov eax, numero
    shl eax, 1
    call WriteDec
    call Crlf

    exit
main ENDP
END main
```

### 13. Práctica 11. Operaciones lógicas (`Practica11_OperacionesLogicas.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 11. Operaciones lógicas
; Descripción: Aplica las operaciones booleanas a nivel de bits (AND, OR, XOR y NOT) sobre dos valores binarios de 8 bits y despliega en consola la representación binaria de cada resultado mediante WriteBinB.

INCLUDE Irvine32.inc

.data
    valA    DWORD 10101100b
    valB    DWORD 00001111b
    msgValA BYTE "Valor A (binario): ", 0
    msgValB BYTE "Valor B (binario): ", 0
    msgAnd  BYTE "Resultado AND:     ", 0
    msgOr   BYTE "Resultado OR:      ", 0
    msgXor  BYTE "Resultado XOR:     ", 0
    msgNot  BYTE "Resultado NOT A:   ", 0

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgValA
    call WriteString
    mov eax, valA
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgValB
    call WriteString
    mov eax, valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf
    call Crlf

    mov edx, OFFSET msgAnd
    call WriteString
    mov eax, valA
    and eax, valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgOr
    call WriteString
    mov eax, valA
    or eax, valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgXor
    call WriteString
    mov eax, valA
    xor eax, valB
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgNot
    call WriteString
    mov eax, valA
    not al
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    exit
main ENDP
END main
```

### 14. Práctica 12. Desplazamiento y rotación (`Practica12_DesplazamientoYRotacion.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 12. Desplazamiento y rotación
; Descripción: Realiza manipulaciones de bits sobre un byte base (10010110b) empleando instrucciones de desplazamiento lógico a la izquierda (SHL) y derecha (SHR), así como rotaciones circulares (ROL y ROR), mostrando cada resultado en binario.

INCLUDE Irvine32.inc

.data
    valorBase BYTE 10010110b
    msgBase   BYTE "Valor original:         ", 0
    msgSHL    BYTE "Desplazamiento SHL 1:   ", 0
    msgSHR    BYTE "Desplazamiento SHR 1:   ", 0
    msgROL    BYTE "Rotacion ROL 2:         ", 0
    msgROR    BYTE "Rotacion ROR 2:         ", 0

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgBase
    call WriteString
    movzx eax, valorBase
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgSHL
    call WriteString
    movzx eax, valorBase
    shl al, 1
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgSHR
    call WriteString
    movzx eax, valorBase
    shr al, 1
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgROL
    call WriteString
    movzx eax, valorBase
    rol al, 2
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    mov edx, OFFSET msgROR
    call WriteString
    movzx eax, valorBase
    ror al, 2
    mov ebx, TYPE BYTE
    call WriteBinB
    call Crlf

    exit
main ENDP
END main
```

### 15. Práctica 13. String hexadecimal (`Practica13_StringHexadecimal.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 13. String hexadecimal
; Descripción: Captura un número entero decimal de 32 bits y lo convierte manualmente a una cadena de texto en formato hexadecimal de 8 dígitos extrayendo grupos de 4 bits (nibbles) mediante desplazamientos SHR y una tabla de búsqueda.

INCLUDE Irvine32.inc

.data
    msgPrompt BYTE "Ingrese un numero entero decimal: ", 0
    msgHexOut BYTE "Cadena hexadecimal generada: ", 0
    tablaHex  BYTE "0123456789ABCDEF"
    strHex    BYTE 8 DUP('0'), "h", 0
    valor     DWORD ?

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgPrompt
    call WriteString
    call ReadDec
    mov valor, eax

    mov ecx, 8
    mov edi, OFFSET strHex + 7
    mov ebx, OFFSET tablaHex

ConvertirHex:
    mov edx, eax
    and edx, 0Fh
    mov dl, [ebx + edx]
    mov [edi], dl
    shr eax, 4
    dec edi
    loop ConvertirHex

    mov edx, OFFSET msgHexOut
    call WriteString
    mov edx, OFFSET strHex
    call WriteString
    call Crlf

    exit
main ENDP
END main
```

### 16. Práctica 14. Captura y almacenamiento de dato numérico (`Practica14_CapturaYAlmacenamientoNumerico.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 14. Captura y almacenamiento de dato numérico
; Descripción: Solicita al usuario 5 valores numéricos enteros, los almacena secuencialmente en un arreglo de 32 bits utilizando direccionamiento indirecto por registro ([esi]) y luego recorre el arreglo para mostrar todos los elementos guardados.

INCLUDE Irvine32.inc

.data
    MAX_ELEM   = 5
    arreglo    SDWORD MAX_ELEM DUP(?)
    msgPrompt  BYTE "Ingrese un dato numerico para almacenar: ", 0
    msgMostrar BYTE "Datos numericos almacenados en el arreglo:", 13, 10, 0
    msgSep     BYTE "  ", 0

.code
main PROC
    call Clrscr

    mov ecx, MAX_ELEM
    mov esi, OFFSET arreglo

CicloCaptura:
    mov edx, OFFSET msgPrompt
    call WriteString
    call ReadInt
    mov [esi], eax
    add esi, TYPE SDWORD
    loop CicloCaptura

    call Crlf
    mov edx, OFFSET msgMostrar
    call WriteString

    mov ecx, MAX_ELEM
    mov esi, OFFSET arreglo

CicloDespliegue:
    mov eax, [esi]
    call WriteInt
    mov edx, OFFSET msgSep
    call WriteString
    add esi, TYPE SDWORD
    loop CicloDespliegue

    call Crlf
    exit
main ENDP
END main
```

### 17. Práctica 15. Manipulación de archivo (`Practica15_ManipulacionDeArchivo.asm`)

```masm
; Materia: Lenguajes de Interfaz
; Alumno: José Mario Carrasco Larios
; Horario: 8-9
; Docente: Dr. José Luis Medina Jiménez
; Práctica: Práctica 15. Manipulación de archivo
; Descripción: Captura una línea de texto desde la consola, crea un archivo de salida llamado 'datos_practica15.txt' mediante CreateOutputFile, escribe el contenido capturado usando WriteToFile y cierra el manejador del archivo con CloseFile.

INCLUDE Irvine32.inc

.data
    nombreArchivo BYTE "datos_practica15.txt", 0
    msgPrompt     BYTE "Ingrese el texto a guardar en el archivo: ", 0
    msgExito      BYTE "Archivo creado y escrito correctamente.", 0
    msgError      BYTE "Error al crear el archivo.", 0
    buffer        BYTE 256 DUP(0)
    longitud      DWORD ?
    manejador     HANDLE ?
    bytesEscritos DWORD ?

.code
main PROC
    call Clrscr

    mov edx, OFFSET msgPrompt
    call WriteString

    mov edx, OFFSET buffer
    mov ecx, SIZEOF buffer - 1
    call ReadString
    mov longitud, eax

    mov edx, OFFSET nombreArchivo
    call CreateOutputFile
    mov manejador, eax

    cmp eax, INVALID_HANDLE_VALUE
    je ErrorArchivo

    mov eax, manejador
    mov edx, OFFSET buffer
    mov ecx, longitud
    call WriteToFile
    mov bytesEscritos, eax

    mov eax, manejador
    call CloseFile

    mov edx, OFFSET msgExito
    call WriteString
    call Crlf
    jmp Salir

ErrorArchivo:
    mov edx, OFFSET msgError
    call WriteString
    call Crlf

Salir:
    exit
main ENDP
END main
```
