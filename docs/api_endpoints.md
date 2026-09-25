 # Arquitectura del Sistema - DILIVIRI

## 1. Descripción general

DILIVIRI es una aplicación móvil de comida a domicilio que permite a los clientes consultar restaurantes, visualizar productos, realizar pedidos y consultar el estado de sus pedidos.

La aplicación se comunica con un servidor mediante una API para procesar la información de usuarios, restaurantes, productos y pedidos.

## 2. Componentes principales

### Aplicación móvil

Es la interfaz utilizada por el cliente para:

* Registrarse e iniciar sesión.
* Consultar restaurantes.
* Consultar productos.
* Agregar productos al carrito.
* Realizar pedidos.
* Consultar el estado del pedido.

### API / Servidor

Se encarga de recibir y procesar las solicitudes enviadas desde la aplicación móvil.

Entre sus funciones están:

* Autenticación de usuarios.
* Gestión de restaurantes.
* Gestión de productos.
* Gestión de pedidos.
* Procesamiento de información.

### Base de datos

Almacena la información necesaria para el funcionamiento de DILIVIRI, como:

* Usuarios.
* Restaurantes.
* Productos.
* Pedidos.
* Estados de pedidos.

## 3. Flujo general

El cliente utiliza la aplicación móvil para realizar una acción. La aplicación envía la solicitud a la API, la API procesa la información y consulta o modifica los datos almacenados en la base de datos. Finalmente, el servidor devuelve una respuesta a la aplicación móvil.
