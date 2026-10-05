# DAW Project Hub
Una página para conocer las fases del desarrollo y despliegue de una aplicación web.

## Entorno de Desarrollo

- **Versión de Git:** git version 2.43.0
- **Sistema Operativo:** Windows 11 / macOS Sonoma / Ubuntu 22.04 LTS
- **Editor de Código:** Visual Studio Code

## Conceptos sobre SSH y Seguridad

### 1. ¿Qué es SSH?
SSH es un protocolo de red seguro que permite conectar y comunicar dos ordenadores de forma cifrada a través de una red no segura. Se utiliza principalmente para acceder a servidores de forma remota y autorizar operaciones en plataformas como GitHub sin enviar información sensible en texto plano.

### 2. ¿Qué diferencia existe entre una clave pública y una clave privada?
* **Clave pública:** Funciona como un candado abierto. Sirve para cifrar información o verificar firmas, pero no permite descifrar el contenido.
* **Clave privada:** Funciona como la llave física que abre ese candado. Se utiliza para descifrar la información o firmar digitalmente las conexiones.

### 3. ¿Qué clave puede compartirse?
La **clave pública**. Se puede enviar a servidores, subir a servicios como GitHub o compartir libremente con cualquier entidad a la que quieras identificarte.

### 4. ¿Qué clave no debe compartirse nunca?
La **clave privada**. Debe permanecer custodiada y accesible únicamente por el usuario en su máquina local.

### 5. ¿Qué ventaja presenta SSH frente a introducir continuamente usuario y contraseña?
* **Mayor comodidad:** Evita tener que escribir las credenciales manualmente en cada interacción con el servidor (como en cada git push o git pull).
* **Mayor seguridad:** Utiliza algoritmos criptográficos robustos que no viajan por la red en formato de texto plano y resisten ataques de fuerza bruta mucho mejor que las contraseñas tradicionales.

### 6. ¿Qué función cumple el archivo known_hosts?
Es un registro local donde tu equipo guarda la huella digital de los servidores a los que te has conectado previamente mediante SSH. Su función es verificar la identidad del servidor en futuras conexiones para evitar ataques de tipo *Man-in-the-Middle* (donde un tercero intenta suplantar al servidor).

### 7. ¿Qué podría ocurrir si una clave privada se publica en GitHub?
Cualquier persona que la encuentre obtendría acceso total y no autorizado a todos los sistemas, servidores o cuentas de GitHub configurados con su clave pública correspondiente. Esto permitiría a un atacante suplantar tu identidad, modificar o borrar código, o comprometer servidores remotos.

## Conexión SSH con GitHub: comprobada correctamente

Historial del proyecto

El proyecto se ha desarrollado mediante varios commits pequeños y coherentes. Cada commit representa un cambio concreto, como crear la estructura HTML, añadir la cabecera, incorporar la sección principal, escribir los tres párrafos, añadir el pie de página o aplicar los estilos.

Realizar varios commits pequeños facilita el seguimiento de la evolución del proyecto y permite identificar con mayor precisión qué cambios se realizaron en cada momento. También hace más sencillo revisar el código, localizar posibles errores y volver a un estado anterior si fuera necesario.

En cambio, realizar un único commit con toda la página mezcla muchos cambios diferentes en una sola operación, lo que dificulta comprender la evolución del proyecto y revisar o localizar modificaciones concretas. Por ello, es preferible utilizar commits pequeños, coherentes y descriptivos.

## Actualización remota

Este cambio se ha realizado directamente desde GitHub para practicar `fetch` y `pull`.

## Forks y colaboración

### 1. ¿Qué es un fork en GitHub?

Un fork es una copia de un repositorio que se crea dentro de otra cuenta de GitHub. Permite trabajar sobre un proyecto sin modificar directamente el repositorio original.

### 2. ¿En qué se diferencia un fork de una rama?

Una rama pertenece al mismo repositorio y normalmente se utiliza para desarrollar distintas versiones o funcionalidades dentro de ese proyecto. Un fork, en cambio, es una copia del repositorio que pertenece a otra cuenta y funciona como un repositorio independiente.

### 3. ¿En qué cuenta se almacena un fork?

El fork se almacena en la cuenta de GitHub de la persona u organización que lo crea. Por ejemplo, si una persona hace un fork de un proyecto de otra cuenta, la copia aparecerá en su propia cuenta.

### 4. ¿Cuándo resulta útil trabajar mediante un fork?

Es especialmente útil cuando queremos proponer cambios en un proyecto en el que no tenemos permisos para modificar directamente. Podemos trabajar en nuestra propia copia y preparar allí los cambios antes de proponerlos al proyecto original.

### 5. ¿Qué relación existe entre el repositorio original y el fork?

El fork comienza como una copia del repositorio original, pero después puede evolucionar de manera independiente. GitHub mantiene la relación entre ambos para facilitar la colaboración y la propuesta de cambios.

### 6. ¿Qué es el repositorio upstream?

Upstream es el nombre que normalmente se utiliza para identificar el repositorio original del que procede nuestro fork. Sirve como referencia para poder consultar y obtener las actualizaciones que se produzcan en el proyecto original.

### 7. ¿Qué diferencia existe entre origin y upstream?

`origin` suele ser el repositorio remoto principal que tenemos configurado en nuestro clon local. Cuando trabajamos con un fork, normalmente `origin` apunta a nuestro propio fork, mientras que `upstream` apunta al repositorio original.

### 8. ¿Cómo se propone que un cambio del fork llegue al repositorio original?

Primero se realizan los cambios en el fork y se publican en GitHub. Después se crea una Pull Request dirigida al repositorio original. En ella se explican los cambios realizados para que puedan ser revisados.

### 9. ¿Quién decide si se acepta la propuesta?

La decisión corresponde a las personas que mantienen el repositorio original y tienen permisos para revisar y aceptar cambios. Pueden aprobar la Pull Request, solicitar modificaciones o rechazarla.

### 10. ¿Puede seguir evolucionando el repositorio original mientras existe el fork?

Sí. El repositorio original puede continuar recibiendo nuevos commits mientras el fork sigue existiendo. Por eso un fork puede quedarse desactualizado respecto al original y, si queremos continuar trabajando con los cambios más recientes, podemos sincronizarlo con `upstream`.

### Resumen

Un fork permite trabajar sobre una copia propia de un proyecto y proponer cambios al repositorio original sin necesidad de tener permisos de escritura en él. Las ramas sirven para organizar el desarrollo dentro de un repositorio, mientras que el fork separa el trabajo en otro repositorio. Cuando usamos un fork, `origin` suele representar nuestra copia y `upstream` el proyecto original.
