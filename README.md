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
