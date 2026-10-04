# Reportes de errores: Urban Scooter

Listado de bugs registrados en Jira (proyecto USBT).

## Índice

| Clave | Resumen | Entorno |
|---|---|---|
| [USBT-1](#usbt-1) | Búsqueda de pedido no funciona con tecla enter | Microsoft Edge |
| [USBT-2](#usbt-2) | Pedido cancelado puede ser consultado | Microsoft Edge |
| [USBT-3](#usbt-3) | Campo apellido permite más de 15 caracteres | Google Chrome |
| [USBT-4](#usbt-4) | Campo fecha permite reservar para el mismo día | Google Chrome |
| [USBT-5](#usbt-5) | Campo color permite seleccionar ambos colores | Google Chrome |
| [USBT-6](#usbt-6) | Campo comentario permite más de 24 caracteres | Google Chrome |
| [USBT-7](#usbt-7) | Campo comentario permite caracteres especiales | Google Chrome |
| [USBT-8](#usbt-8) | Mensaje usuario o contraseña no válido no aparece | Android emulator |
| [USBT-9](#usbt-9) | No se recibe notificación dos horas antes de tener que completar pedidos | Android emulator |
| [USBT-10](#usbt-10) | Sin conexión el botón filtro no manda mensaje "Sin acceso a Internet" | Android emulator |
| [USBT-11](#usbt-11) | Todos los pedidos, sin conexión no manda mensaje "Sin acceso a Internet" al revisar detalle de pedido | Android emulator |
| [USBT-12](#usbt-12) | Mis pedidos, sin conexión no manda mensaje "Sin acceso a Internet" al revisar detalle de pedido | Android emulator |
| [USBT-13](#usbt-13) | Sin conexión no manda mensaje "Sin acceso a Internet" al hacer click en el botón cerrar sesión | Android emulator |
| [USBT-14](#usbt-14) | Sin conexión no manda mensaje "Sin acceso a Internet" al hacer click en el botón iniciar sesión | Android emulator |
| [USBT-15](#usbt-15) | Sin conexión no manda mensaje "Sin acceso a Internet" al hacer click en el botón "Olvidé la contraseña" | Android emulator |
| [USBT-16](#usbt-16) | No se puede cancelar un pedido | Postman API backend |
| [USBT-17](#usbt-17) | Pedidos siguen apareciendo después de eliminar repartidor | Postman API backend, PostgreSQL |
| [USBT-18](#usbt-18) | No se puede aceptar un pedido | Postman API backend, PostgreSQL |
| [USBT-19](#usbt-19) | Estatus de pedido aceptado no muestra el nombre del repartidor | Microsoft Edge |
| [USBT-20](#usbt-20) | Estatus de pedido aceptado no muestra el nombre del repartidor | Microsoft Edge |
| [USBT-21](#usbt-21) | El estatus del pedido pasa del estado 2 al 4 sin pasar por el 3 | Microsoft Edge |
| [USBT-22](#usbt-22) | El estado 4 no muestra fecha de terminación del alquiler | Mozilla Firefox, Google Chrome |
| [USBT-23](#usbt-23) | El campo dirección no permite escribir 50 caracteres | Mozilla Firefox, Google Chrome |
| [USBT-24](#usbt-24) | El campo comentario permite escribir letras no latinas | Mozilla Firefox, Google Chrome |
| [USBT-25](#usbt-25) | Bad request al cancelar pedido inexistente | Postman API backend |

---

## USBT-1
### Búsqueda de pedido no funciona con tecla enter

**Enlace:** https://esccel21.atlassian.net/browse/USBT-1
**Entorno:** Microsoft Edge

**Pasos para reproducir:**
1. En la pantalla de estado del pedido pegar o escribir número de pedido
2. Presionar enter

**Resultado esperado:** Se muestra el estado del pedido una vez que se presiona la tecla enter.

**Resultado actual:** La página no hace nada.

---

## USBT-2
### Pedido cancelado puede ser consultado

**Enlace:** https://esccel21.atlassian.net/browse/USBT-2
**Entorno:** Microsoft Edge

**Pasos para reproducir:**
1. En la pantalla de estado del pedido pegar o escribir número de pedido
2. Presionar botón “¡Vamos!”

**Resultado esperado:** Se debería mostrar un mensaje de pedido inválido/no encontrado.

**Resultado actual:** La página muestra el estado del pedido como si no se hubiera cancelado.

---

## USBT-3
### Campo apellido permite más de 15 caracteres

**Enlace:** https://esccel21.atlassian.net/browse/USBT-3
**Entorno:** Google Chrome

**Pasos para reproducir:**
1. Entrar al apartado pedir
2. Ingresar nombre
3. Ingresar un apellido que contenga más de 15 caracteres válidos

**Resultado esperado:** Debería mostrar error al ingresar más de 15 caracteres, que es el límite.

**Resultado actual:** Te permite agregar más de 15 caracteres.

---

## USBT-4
### Campo fecha permite reservar para el mismo día

**Enlace:** https://esccel21.atlassian.net/browse/USBT-4
**Entorno:** Google Chrome

**Pasos para reproducir:**
1. Entrar al apartado pedir
2. Ingresar todos los campos hasta llegar a la pantalla de alquiler
3. Ingresar fecha del mismo día

**Resultado esperado:** Debería mostrar error ya que solo se deberían permitir fechas futuras.

**Resultado actual:** Te permite seleccionar la fecha actual o fechas pasadas.

---

## USBT-5
### Campo color permite seleccionar ambos colores

**Enlace:** https://esccel21.atlassian.net/browse/USBT-5
**Entorno:** Google Chrome

**Pasos para reproducir:**
1. Entrar al apartado pedir
2. Ingresar todos los campos hasta llegar a la pantalla de alquiler
3. Seleccionar ambas opciones en el campo “El color del scooter”

**Resultado esperado:** Debería mostrar error ya que solo se debería permitir un color.

**Resultado actual:** Te permite seleccionar ambas opciones de color.

---

## USBT-6
### Campo comentario permite más de 24 caracteres

**Enlace:** https://esccel21.atlassian.net/browse/USBT-6
**Entorno:** Google Chrome

**Pasos para reproducir:**
1. Entrar al apartado pedir
2. Ingresar todos los campos hasta llegar a la pantalla de alquiler
3. Ingresar un comentario con más de 24 caracteres

**Resultado esperado:** Debería mostrar error ya que debería tener un límite de 24 caracteres.

**Resultado actual:** Te permite agregar más de 24 caracteres.

---

## USBT-7
### Campo comentario permite caracteres especiales

**Enlace:** https://esccel21.atlassian.net/browse/USBT-7
**Entorno:** Google Chrome

**Pasos para reproducir:**
1. Entrar al apartado pedir
2. Ingresar todos los campos hasta llegar a la pantalla de alquiler
3. Ingresar un comentario con caracteres especiales

**Resultado esperado:** Debería mostrar error ya que no debería permitir caracteres especiales.

**Resultado actual:** Te permite agregar caracteres especiales.

---

## USBT-8
### Mensaje usuario o contraseña no válido no aparece

**Enlace:** https://esccel21.atlassian.net/browse/USBT-8
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario incorrecto y contraseña

**Resultado esperado:** Debería mostrar recuadro con mensaje “usuario o contraseña inválido”.

**Resultado actual:** Muestra leyenda `HTTP 404 Not Found`.

---

## USBT-9
### No se recibe notificación dos horas antes de tener que completar pedidos

**Enlace:** https://esccel21.atlassian.net/browse/USBT-9
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario y contraseña
3. Aceptar pedido

**Resultado esperado:** Debería mostrar una notificación dos horas antes de terminar el día en que se debe completar el pedido.

**Resultado actual:** No se recibe notificación.

---

## USBT-10
### Sin conexión el botón filtro no manda mensaje "Sin acceso a Internet"

**Enlace:** https://esccel21.atlassian.net/browse/USBT-10
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario y contraseña
3. Poner dispositivo en modo avión o desconectar de cualquier conexión a internet
4. Ir a pestaña “Todos los pedidos”
5. Click en botón filtro (dos líneas al lado de “Lista de pedidos”)

**Resultado esperado:** Debería mostrar un mensaje en pantalla “Sin acceso a Internet”.

**Resultado actual:** Te permite ver los filtros.

---

## USBT-11
### Todos los pedidos, sin conexión no manda mensaje "Sin acceso a Internet" al revisar detalle de pedido

**Enlace:** https://esccel21.atlassian.net/browse/USBT-11
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario y contraseña
3. Poner dispositivo en modo avión o desconectar de cualquier conexión a internet
4. Ir a pestaña “Todos los pedidos”
5. Click en cualquier pedido

**Resultado esperado:** Debería mostrar un mensaje en pantalla “Sin acceso a Internet”.

**Resultado actual:** Te permite ver el detalle del pedido.

---

## USBT-12
### Mis pedidos, sin conexión no manda mensaje "Sin acceso a Internet" al revisar detalle de pedido

**Enlace:** https://esccel21.atlassian.net/browse/USBT-12
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario y contraseña
3. Poner dispositivo en modo avión o desconectar de cualquier conexión a internet
4. Ir a pestaña “Mis pedidos”
5. Click en cualquier pedido

**Resultado esperado:** Debería mostrar un mensaje en pantalla “Sin acceso a Internet”.

**Resultado actual:** Te permite ver el detalle del pedido.

---

## USBT-13
### Sin conexión no manda mensaje "Sin acceso a Internet" al hacer click en el botón cerrar sesión

**Enlace:** https://esccel21.atlassian.net/browse/USBT-13
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario y contraseña
3. Poner dispositivo en modo avión o desconectar de cualquier conexión a internet
4. Click en el botón cerrar sesión

**Resultado esperado:** Debería mostrar un mensaje en pantalla “Sin acceso a Internet”.

**Resultado actual:** Muestra mensaje “¿Deseas cerrar sesión?”.

---

## USBT-14
### Sin conexión no manda mensaje "Sin acceso a Internet" al hacer click en el botón iniciar sesión

**Enlace:** https://esccel21.atlassian.net/browse/USBT-14
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario y contraseña
3. Poner dispositivo en modo avión o desconectar de cualquier conexión a internet
4. Click en el botón iniciar sesión

**Resultado esperado:** Debería mostrar un mensaje en pantalla “Sin acceso a Internet”.

**Resultado actual:** Muestra leyenda en la parte inferior de la pantalla “Unable to resolve host “cnt…”.

---

## USBT-15
### Sin conexión no manda mensaje "Sin acceso a Internet" al hacer click en el botón "Olvidé la contraseña"

**Enlace:** https://esccel21.atlassian.net/browse/USBT-15
**Entorno:** Android emulator

**Pasos para reproducir:**
1. Iniciar aplicación
2. Ingresar usuario y contraseña
3. Poner dispositivo en modo avión o desconectar de cualquier conexión a internet
4. Click en el botón “Olvidé la contraseña”

**Resultado esperado:** Debería mostrar un mensaje en pantalla “Sin acceso a Internet”.

**Resultado actual:** Muestra mensaje en pantalla “Contacte a la gerencia: 0101”.

---

## USBT-16
### No se puede cancelar un pedido

**Enlace:** https://esccel21.atlassian.net/browse/USBT-16
**Entorno:** Postman API backend

**Pasos para reproducir:**
1. Iniciar Postman
2. Ingresar endpoint y cuerpo de la solicitud:
   - Endpoint: `{{base_url}}/api/v1/orders/cancel`
   - Cuerpo:
     ```json
     {
         "track": 123757
     }
     ```
3. Enviar solicitud

**Resultado esperado:** Debería mostrar código `200 OK`.

**Resultado actual:** Muestra código `400 Bad Request`.

---

## USBT-17
### Pedidos siguen apareciendo después de eliminar repartidor

**Enlace:** https://esccel21.atlassian.net/browse/USBT-17
**Entorno:** Postman API backend, PostgreSQL database

**Pasos para reproducir:**
1. Iniciar Postman
2. Ingresar endpoint y cuerpo de la solicitud:
   - Endpoint: `{{base_url}}/api/v1/courier`
   - Cuerpo:
     ```json
     {
         "login": "felix",
         "password": "1234",
         "firstName": "fe"
     }
     ```
3. Enviar solicitud
4. Revisar tabla “Orders” en base de datos

**Resultado esperado:** Los pedidos asignados al courier eliminado ya no deberían estar.

**Resultado actual:** Los pedidos siguen apareciendo.

---

## USBT-18
### No se puede aceptar un pedido

**Enlace:** https://esccel21.atlassian.net/browse/USBT-18
**Entorno:** Postman API backend, PostgreSQL database

**Pasos para reproducir:**
1. Iniciar Postman
2. Ingresar endpoint con los parámetros de orden y repartidor:
   - `{{base_url}}/api/v1/orders/accept/648061?courierId=3`
3. Enviar solicitud

**Resultado esperado:** `200 OK` y el pedido debería cambiar a status 1.

**Resultado actual:** `404 Not Found`, y el pedido no cambia de status.

```json
{
    "code": 404,
    "message": "There's no order with this ID."
}
```

---

## USBT-19
### Estatus de pedido aceptado no muestra el nombre del repartidor

**Enlace:** https://esccel21.atlassian.net/browse/USBT-19
**Entorno:** Microsoft Edge

**Pasos para reproducir:**
1. En la pantalla de estado del pedido pegar o escribir número de pedido
2. Aceptar el pedido en la aplicación móvil

**Resultado esperado:** Se muestra el estado del pedido "en camino" con el nombre del repartidor.

**Resultado actual:** Se muestra mensaje sin nombre del repartidor.

---

## USBT-20
### Estatus de pedido aceptado no muestra el nombre del repartidor

**Enlace:** https://esccel21.atlassian.net/browse/USBT-20
**Entorno:** Microsoft Edge

**Pasos para reproducir:**
1. En la pantalla de estado del pedido pegar o escribir número de pedido
2. Presionar enter

**Resultado esperado:** Se muestra el estado del pedido una vez que se presiona la tecla enter.

**Resultado actual:** La página no hace nada.

> ⚠️ La descripción de este ticket coincide con la de USBT-1 y no con su resumen (ver USBT-19).

---

## USBT-21
### El estatus del pedido pasa del estado 2 al 4 sin pasar por el 3

**Enlace:** https://esccel21.atlassian.net/browse/USBT-21
**Entorno:** Microsoft Edge

**Pasos para reproducir:**
1. En la pantalla de estado del pedido pegar o escribir número de pedido
2. Aceptar el pedido en la aplicación móvil
3. Completar el pedido en la aplicación móvil

**Resultado esperado:** Se muestra el estado del pedido con el mensaje “El servicio de entrega llegó”.

**Resultado actual:** Se muestra mensaje “Bien, vamos a dar un paseo”.

---

## USBT-22
### El estado 4 no muestra fecha de terminación del alquiler

**Enlace:** https://esccel21.atlassian.net/browse/USBT-22
**Entorno:** Mozilla Firefox, Google Chrome

**Pasos para reproducir:**
1. En la pantalla de estado del pedido pegar o escribir número de pedido
2. Aceptar el pedido en la aplicación móvil
3. Completar el pedido en la aplicación móvil

**Resultado esperado:** Se muestra el estado del pedido con el mensaje:
> “Bien, vamos a dar un paseo
> El alquiler terminará el 02.10.2026”

**Resultado actual:** Se muestra el mensaje:
> “Bien, vamos a dar un paseo
> El alquiler terminará el `{{data}}`”

---

## USBT-23
### El campo dirección no permite escribir 50 caracteres

**Enlace:** https://esccel21.atlassian.net/browse/USBT-23
**Entorno:** Mozilla Firefox, Google Chrome

**Pasos para reproducir:**
1. Hacer click en el botón “Pedir”
2. Ingresar un nombre válido
3. Ingresar un apellido válido
4. Ingresar una dirección con al menos 50 caracteres

**Resultado esperado:** Se valida la dirección con éxito sin mostrar error, ya que el límite es 50.

**Resultado actual:** Se muestra mensaje “Introduce un número válido”.

---

## USBT-24
### El campo comentario permite escribir letras no latinas

**Enlace:** https://esccel21.atlassian.net/browse/USBT-24
**Entorno:** Mozilla Firefox, Google Chrome

**Pasos para reproducir:**
1. Hacer click en el botón “Pedir”
2. Ingresar un nombre válido
3. Ingresar un apellido válido
4. Ingresar una dirección válida
5. Seleccionar una estación de metro
6. Ingresar un teléfono válido
7. Dar click en siguiente
8. Seleccionar fecha
9. Seleccionar periodo del alquiler
10. Ingresar comentario con letras no latinas

**Resultado esperado:** Se valida la dirección con éxito sin mostrar error ya que solo debería permitir letras latinas.

**Resultado actual:** Se puede continuar con el pedido aún con el comentario en letras no latinas.

---

## USBT-25
### Bad request al cancelar pedido inexistente

**Enlace:** https://esccel21.atlassian.net/browse/USBT-25
**Entorno:** Postman API backend

**Pasos para reproducir:**
1. Iniciar Postman
2. Ingresar endpoint y cuerpo de la solicitud con un número de pedido inexistente:
   - Endpoint: `{{base_url}}/api/v1/orders/cancel`
   - Cuerpo:
     ```json
     {
         "track": 412365
     }
     ```
3. Enviar solicitud

**Resultado esperado:** Debería mostrar código `404 Not Found`.

**Resultado actual:** Muestra código `400 Bad Request`.
