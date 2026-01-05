# Paquete-MW-MW-Package-Win-Anti-App-Anchor-1-MAWA-Trity-and-MW-Console
En este repositorio publicare TODO sobre mis proyectos, soy Samuel Leonardo Páez garzón, y este README te gustara Gracias.

Me llamo Samuel Leonardo Páez Garzón Soy un niño de 13 años con Asperger que sueña con mejorar el bajo nivel presentando a MAWA como una solución a su complejidad dado a que Ensamblador es algo complejo para algunas personas y puede no llamarles la atención ver ese lenguaje tan extraño en sintaxis, es normal ya que no están familiarizados con él, entonces aquí llega MAWA como una solución con una sintaxis simple y para nada compleja similar en facilidad a la de Python pero permitiendote generar código máquina para bootloaders, kernels, o incluso todo tu proyecto de bajo nivel, etc...

Procedo a mostrarles a MAWA:

Si quieren seguir mi proceso en mis proyectos de manera más directa pueden ir a Dev.To y buscarme como Samuel Leonardo Páez Garzón o seguirme en Youtube como Mi Ancla Oficial VIDSLPG

En este POST explico el funcionamiento del comando Imp es un post de Dev.To, si lo quieres leer entra a este link:
https://dev.to/samuel_leonardo_37aff38b4/mawa-el-lenguaje-simple-de-bajo-nivel-parte-2-probando-mi-lenguaje-2enj

Estructura de un archivo del lenguaje en la librería MWBN:
Este es un código de ejemplo puedes inferir que hace o leer los comentarios para saberlo explicitamente.

```python
ARQ 16 ; Aquí declaras en que tecnología usarás MAWA
DIR 0x7C00 ; Aquí declaras donde cargas tu código para que MAWA cargue las direcciones de variables o otras cosas en esa dirección

String (Nombre) = "Samuel Leonardo Páez Garzón" ; Aquí creo una variable
Imp ("Hola ", Nombre, 0x04) ; Aquí imprimo la cadena "Hola" y la variable en color rojo
InfiniteLoop() ; Esto hace un bucle infinito para no seguir avanzando en NASM sería jmp $

#Add (ALL/MWBN) ; Esto incrusta las funciones de MAWA en el archivo si está línea no está el código no te funcionara

Instruction(Rellenar-510) ; Esto rellena a 510 Bytes el archivo necesario si es un BootLoader
Insert Bytes16(0xAA55) ; Esto inserta la firma de arranque 55 AA también este comando se vale por Insert WORD(0xAA55)
```

Funcionamiento del Imp:
La función de Imp es imprimir algo revolucionario inicial es que mientras que en MAWA imprimir Hola Mundo es:
```mawa
Imp ("Hola Mundo")
```

En Ensamblador secuencia NASM es:
```asm
mov si, mensaje
call imprimirCadena

imprimirCadena:
    lodsb
    or al, al
    jz impresionHecha
    mov ah, 0x0E
    int 0x10
    jmp imprimirCadena
impresionHecha:
    ret

mensaje db "Hola Mundo", 0
```

Como te pudiste dar cuenta la simplicidad es bastante de MAWA VS Assembler (Alias Ensamblador)

Bueno aquí les mostre una pizquita de todo MAWA si quieren ver más en un futuro públicare mi documentación del lenguaje en un futuro para ue vean todos los comandos.

Samuel Leomardo Páez Garzón - 2026/2027
Todos los derechos de autor reservados.


