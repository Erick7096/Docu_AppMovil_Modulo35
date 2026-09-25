# Políticas de Seguridad de la Aplicación Móvil

## 1. Autenticación

DILIVIRI utiliza autenticación para controlar el acceso de los usuarios a las funciones de la aplicación.

El usuario debe proporcionar sus credenciales para acceder a las funciones protegidas.

## 2. Almacenamiento Local Seguro

Los tokens de sesión no deben almacenarse en texto plano.

La aplicación debe utilizar mecanismos de almacenamiento seguro proporcionados por el sistema operativo móvil.

En Android puede utilizarse un mecanismo como EncryptedSharedPreferences y en iOS Keychain, según corresponda a la implementación.

## 3. Protección de Credenciales

Las contraseñas y credenciales del usuario no deben almacenarse directamente dentro de la aplicación.

La autenticación debe realizarse mediante el servidor.

## 4. Comunicación con la API

La aplicación debe utilizar comunicaciones seguras con el servidor para proteger la información transmitida.

## 5. Permisos del Dispositivo

La aplicación únicamente debe solicitar los permisos estrictamente necesarios.

Los permisos deben solicitarse en tiempo de ejecución cuando corresponda.

## 6. Ubicación

Si DILIVIRI utiliza la ubicación para facilitar la entrega de pedidos, el permiso de ubicación debe solicitarse únicamente cuando sea necesario.

## 7. Notificaciones

Si DILIVIRI utiliza notificaciones para informar cambios en los pedidos, el permiso correspondiente debe solicitarse de acuerdo con las capacidades del sistema operativo.

## 8. Protección de la Información

La información de los usuarios, pedidos, direcciones y demás datos debe manejarse de forma segura y únicamente para las funciones necesarias de la aplicación.