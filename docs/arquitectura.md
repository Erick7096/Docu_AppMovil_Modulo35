# Arquitectura del Sistema - DILIVIRI

## 1. Descripción General

DILIVIRI es una aplicación móvil de comida a domicilio que permite a los clientes consultar restaurantes, visualizar productos, agregar productos al carrito, realizar pedidos y consultar el estado de sus pedidos.

La aplicación móvil se comunica con un servidor mediante una API REST para enviar y recibir información.

## 2. Componentes del Sistema

### 2.1 Aplicación Móvil

Es la interfaz principal utilizada por el cliente.

Permite:

- Registrarse e iniciar sesión.
- Consultar restaurantes.
- Consultar productos.
- Agregar productos al carrito.
- Realizar pedidos.
- Consultar el estado del pedido.
- Consultar el historial de pedidos.
- Recibir notificaciones.

### 2.2 Servicio / Controlador Móvil

Se encarga de controlar las acciones realizadas desde la interfaz móvil y preparar las solicitudes que serán enviadas al servidor.

### 2.3 API REST

La API recibe las solicitudes HTTP enviadas por la aplicación móvil.

Entre sus funciones se encuentran:

- Autenticación de usuarios.
- Consulta de restaurantes.
- Consulta de productos.
- Creación de pedidos.
- Actualización del estado de los pedidos.
- Gestión de usuarios.

### 2.4 Base de Datos

Almacena la información necesaria para el funcionamiento del sistema.

Entre los datos almacenados se encuentran:

- Usuarios.
- Restaurantes.
- Productos.
- Pedidos.
- Detalles de pedidos.
- Direcciones de entrega.
- Estados de pedidos.

### 2.5 Restaurante

El restaurante recibe los pedidos realizados por los clientes y gestiona su preparación.

### 2.6 Repartidor

El repartidor recoge el pedido en el restaurante y lo entrega al cliente.

## 3. Flujo General

1. El cliente utiliza la aplicación móvil.
2. La aplicación procesa la acción solicitada.
3. El servicio móvil genera una solicitud HTTP.
4. La solicitud es enviada a la API REST.
5. La API procesa la información.
6. La API consulta o modifica la base de datos.
7. La API devuelve una respuesta.
8. La aplicación móvil muestra el resultado al cliente.