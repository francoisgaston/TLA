# TPE_TLA
## The L programming language

#### Una extensión del proyecto [Flex-Bison-Compiler](https://github.com/agustin-golmar/Flex-Bison-Compiler) 
<hr>

## Compilación
Para construir el compilador, ejecutar en la raíz del proyecto los siguientes comandos

```bash
chmod u+x --recursive script
script/build.sh
```

## Testing
Para correr los programas de testeo (que se pueden encontar en `test/`), ejecutar el siguiente comando
```bash
script/test.sh
```

## Ejecución 
Si se desea correr al compilador con un programa (como `test/accept/01-simplecircuit`), ejecutar el siguiente comando
```bash
script/start.sh test/accept/01-SimpleCircuit
```
Si se desea eliminar a la salida de logs cuando se ejecuta, se debe comentar la siguiente línea en `src/backend/support/logger.h`
```c
#define DEBUG true
```

### Archivo de salida
Es posible indicar el nombre del archivo donde se desea guardar la compilación.
Para ello, se debe agregar un segundo parámetro al comando anterior, indicando el nombre del archivo de salida.
```bash
script/start.sh test/accept/01-SimpleCircuit out.py
```
En este caso, la compilación se guardará en el archivo `out.py`.
<br>
<br>
Si no se indica el nombre del archivo de salida, se guardará en `salida.py` por defecto.
