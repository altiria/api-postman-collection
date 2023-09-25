# Colección Postman para la APIs de Altiria
![](https://img.shields.io/badge/version-1.0.0-blue.svg)

Este repositorio contiene la colección de Postman para las APIs de Altiria. Está constituido por dos ficheros: <br/>
- **API_Altiria_SMS.postman_collection.json**: contiene la colección de Postman y su documentación.<br/>
- **API_Altiria_SMS.postman_environment.json**: contiene las variables de entorno.

Para probar la colección es necesario importar ambos ficheros en la aplicación Postman.
Para poder ejecutar esta colección de peticiones satisfactoriamente, es necesario configurar los valores parametrizados en la sección "Environments" del menú lateral izquierdo. Para esto, primero habrá que importar el archivo API_Altiria_SMS.postman_environment.json. A continuación, será necesario fijar el valor deseado en la columna CURRENT VALUE para cada uno de los campos. En el caso del parámetro URL_BASE, no es necesario realizar ninguna modificación salvo que quiera realizarse la petición sin SSL. Para que estos valores se hagan efectivos se debe activar el checkbox "Set active" en las variables importadas.
No obstante, si no se desea importar este archivo, tendrán que sustituirse las parametrizaciones realizadas en las peticiones una a una manualmente. Estas se identifican fácilmente al mostrarse entre doble llave. En cualquier caso, no recomendamos esta opción.

En esta colección se prueba cada característica por separado con el objetivo de simplificar al máximo cada prueba. Sin embargo, pueden combinarse los diferentes parámetros según la necesidad. Por ejemplo, para realizar un envío de SMS concatenado con codificación unicode y solicitando la confirmación de entrega, utilizaremos los parámetros "concat", "encoding" y "ack" simultáneamente.
Si durante las pruebas se presentan problemas, se recomienda revisar el manual técnico de la API en cuestión.

Para más información, se puede consultar la documentación haciendo clic derecho sobre la misma en el menú lateral izquierdo y seleccionando "View documentation". También se recomienda revisar los manuales técnicos:<br/>
https://www.altiria.com/api-envio-sms/
