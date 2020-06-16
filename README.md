# Drive_PR4
Coltrolador de impresora 4 en 1 por hexadecimal Olivetti PR4 S

Software para controlar la impresora Olivetti PR4 en sus cuatro funciones.
1. Rollo de diario;
2. Rollo de recibos; 
3. Pepel de deslizamiento;
4. Papel de deslizamiento de validación;

Antes de ejecutar en Windows.
Instalar impresora con controlador "Gnerico solo texto" y compartirla.
Obtener la ruta de la impresora o cola de impresión (Ejemplo en windows: \\MaquinaLuis\OlivettiPR4).
Tener Java instalado o bien tener el jre portable.

Forma de Ejecutarlo (Ejemplo de impresion de "Hola Mundo" en  Pepel de deslizamiento):
Desde la consola de windows.
java -jar Driver_PR4.jar "ex" "\\MaquinaLuis\OlivettiPR4" "ESC" "0x1B,0x63,0x30,0x04" <enter>
java -jar Driver_PR4.jar "ex" "\\MaquinaLuis\OlivettiPR4" "STR" "Hola Mundo" <enter>
java -jar Driver_PR4.jar "ex" "\\MaquinaLuis\OlivettiPR4" "ESC" "0x0C" <enter>
