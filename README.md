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