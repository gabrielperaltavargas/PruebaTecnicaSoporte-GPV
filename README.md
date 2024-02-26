## Prueba técnica para el cargo de Soporte

Versión de Prueba Resuelta por Gabriel Peralta Vargas!

Además de lo siempre para iniciar un proyecto Laravel (Aplicar el comando "composer install" para agregar todos los archivos de compose necesarios y faltantes). A grandes rasgos el Código poseía 7 errores:

1. En web.php, erróneamente estaba escrita una función Post en lugar de una Get.

2. En el archivo de View, estaba asignado como "diplay: none" en lugar de algo como "display: block". Además de otros errores de sintaxis, como la forma que se referia a la variable enviada a esta View, como algunos Heading tags mal cerrados.

3. En el Controlador, el dentro del Array, la variable Nivel no empezaba en el numero correcto.

4. En el controlador el ciclo While no estaba correctamente definido (estaba escrito como despues de 10 en lugar de hasta 10).

5. En el controlador, no se traspasaba la variable $aplicante, cuando era necesario retornar tanto 'prueba' como $aplicante.

6. En el controlador, en la función entrenar incorrectamente se inicializaba a $aplicante como un Int, cuando este correspondía a un Array dada la definición anterior. 

7. En la función evaluar, la cual recibía el array de $aplicante, la sintaxis era incorrecta, y se supone que el proceso continué hasta que se alcanza un nivel mayor o igual a 10. 

Con todo esto, se encuentra la prueba resuelta

Añadido también cierto toque personal a la vista por parte de su servidor. 

### IMPORTANTE RECORDAR. 

Para probar el proyecto locamente en Localhost antes de inicializarlo, es importante añadir el archivo ".env" correspondiente, con "APP_KEY" propia, o de lo contrario se obtendría un error 500 de servidor (Normalmente se considera mala práctica incluir archivo .env en Repositorio Publico, por ende estos se tienden a mantener privados).

Gracias por su tiempo!! 

Saludos. 