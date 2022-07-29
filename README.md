# Consumo de la API de Face de los coginitive Services de Azure 
**Objetivo:** Crear un programa de reconocimiento de edad por medio de inteligencia artificial.   

![](/imagenes/cognitive_.jpg)

**Requisitos**
- Cuenta de Azure con una suscripción activa
- Equipo de cómputo con sistema operativo: Windows, Linux o MacOs.

**Pasos**  
Ingresamos a la página de ml.Azure.com e iniciamos sesión  
Seleccionamos la opción de crear un área de trabajo.
En la ventana que se abrió del lado derecho llamada Crear un área de trabajo nueva llenamos los siguientes datos:
Nombre del área de trabajo: Colocamos queramos que se llame el área de trabajo.
Suscripción: La suscripción que queramos usar.
Grupo de recursos: Podemos crear uno o seleccionar uno ya existente.
Región: Podemos escoger cualquiera, pero si no queremos que haya mucha latencia escogemos uno cercano a donde vivimos.

Para terminar, damos clic en crear.
![Imagen 1](/imagenes/Imagen1.png)

Damos clic en ir a área de trabajo del área que acabamos de crear.
En el menú de la izquierda seleccionamos proceso.
En la pestaña de instancia de proceso seleccionamos nuevo.
En creación de instancia de proceso, llenamos los siguiente:
Nombre del proceso: Colocamos el que queramos.
Ubicación: Podemos escoger cualquiera.
Tipo de máquina virtual: Seleccionamos la que prefiramos. 
Tamaño de la máquina virtual: Seleccionamos el que queramos.
Para terminar, le damos en crear.
Nota: Instancia de proceso es una forma de decir máquina virtual.
![](/imagenes/Imagen2.png)

Cuando se termine de crear nuestra instancia de proceso, en el menú de la izquierda seleccionamos Notebooks.
En la ventana que se nos abrió en el centro, damos clic en el signo adentro de un círculo. Al dar clic en el signo seleccionamos la opción que dice crear archivo.
![](/imagenes/Imagen3.png)

En el menú que se abrió colocamos el nombre del archivo y dejamos la extensión que tiene por defecto. Y le damos clic en crear.
![](/imagenes/Imagen4.png)

Ingresamos a este link: https://github.com/josejesusguzman/face-api-consumption-python.
Ahí buscamos en el apartado de requerimiento el texto de código de Python explicado.
Seleccionamos el código que se encuentra ahí y lo pegamos en el Notebook.
![](/imagenes/Imagen5.png)

Buscamos la imagen de una persona en internet y copiamos la url de esa imagen, la pegamos en el código que copiamos anteriormente, en esta parte: image_url = 'AQUÍ_PONES_TU_IMAGEN' , en medio de las comillas simples. 
![](/imagenes/Imagen6.png)

Se inicia sesión en Portal.Azure.com
En la barra de búsqueda escribimos “API de Face” y lo seleccionamos.
Damos clic en el apartado crear.
En la pestaña datos básicos, llenamos lo siguiente:

**En Detalles del proyecto**
Suscripción: La suscripción que queramos utilizar.
Grupo de recursos: Podemos crear uno o seleccionar uno ya existente.

**En Detalles de la instancia**
Región: Podemos escoger cualquiera, pero si no queremos que haya mucha latencia escogemos uno cercano a donde vivimos. 
Nombre: Colocamos el que queramos.
Plan de tarifa: Seleccionamos el gratis.
Marcamos la casilla que se encuentra.

Para terminar, damos clic en el botón de revisar y crear, y luego en crear. 
![](/imagenes/Imagen7.png)

Cuando se termine de crear nuestro recurso, en el menú de la parte de la izquierda le damos clic en la opción de claves y puntos de conexión, y copiamos la clave 1.
![](/imagenes/Imagen8.png)

Nos vamos al Notebook y pegamos la clave 1 en la siguiente parte:
subscription_key = "AQUÍ_PONES_TU_CLAVE_DEL_RECURSO_DE_AZURE", nos vamos a Azure y copiamos la url que está en el apartado de extremo y lo pegamos en la siguiente parte:
face_api_url = "AQUÍ_PONES_TU_URL_DESTINO_DEL_RECURSO_DE_AZURE". 
![](/imagenes/Imagen9.png)

Hecho todo esto lo ejecutamos y vemos el resultado que nos arroja.
![](/imagenes/Imagen10.png)