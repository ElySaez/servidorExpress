# README - Aplicación de Gestión de Productos

Este repositorio contiene una sencilla aplicación Node.js para gestionar y recuperar información de productos. La funcionalidad principal está implementada en dos archivos principales: `ProductManager.js` y `app.js`. Además, hay un archivo JSON de muestra llamado `products.json` que almacena los datos de los productos.

## Tabla de Contenidos
- [Instalación](#instalación)
- [Uso](#uso)
- [Puntos de Acceso](#puntos-de-acceso)
- [Datos de Muestra](#datos-de-muestra)
- [Contribuciones](#contribuciones)
- [Licencia](#licencia)

## Instalación

1. Clona este repositorio en tu máquina local.

```shell
git clone https://github.com/ElySaez/servidorExpress
````
2. Navega hasta el directorio del proyecto.
```shell
cd .\servidorExpress-main\
````
3. Instala las dependencias necesarias.
```shell
npm install
````
## Uso
Para iniciar la aplicación, ejecuta el siguiente comando:
```shell
nodemon ./src/app.js
````
o
```shell
node .\src\app.js
````
## Puntos de Acceso

### 1. Obtener Productos

- **URL:** `/productos`
- **Método:** `GET`
- **Descripción:** Devuelve una lista de productos. Opcionalmente, puedes especificar el parámetro de consulta `limit` para limitar el número de resultados. Por ejemplo, `/productos?limit=2` devolverá los dos primeros productos de la lista.
- **Respuesta:** Un arreglo JSON que contiene objetos de productos.

### 2. Obtener Producto por ID

- **URL:** `/productos/:pid`
- **Método:** `GET`
- **Descripción:** Recupera un producto por su ID único. Reemplaza `:pid` con el ID del producto deseado.
- **Respuesta:** Un objeto JSON que representa el producto si se encuentra, o un mensaje de error si no se encuentra.

### 3. Raíz

- **URL:** `/`
- **Método:** `GET`
- **Descripción:** Muestra un mensaje de bienvenida.

### 4. 404 Página no Encontrada

- **URL:** Cualquier punto de acceso no especificado anteriormente
- **Método:** `GET`
- **Descripción:** Muestra un mensaje de "404 Página no Encontrada" para rutas no definidas.

## Datos de Muestra

Los datos de muestra de los productos se almacenan en el archivo `products.json`. Puedes modificar este archivo para agregar, actualizar o eliminar productos. La aplicación leerá y escribirá datos en este archivo.

## Contribuciones

Las contribuciones a este proyecto son bienvenidas. Si tienes sugerencias para mejoras o deseas informar sobre un error, por favor abre un problema o crea una solicitud de extracción (pull request).

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Siéntete libre de usar, modificar y distribuirlo según sea necesario.
