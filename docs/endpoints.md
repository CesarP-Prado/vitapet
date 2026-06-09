[⬅️ Volver al Inicio](../README.md) | [📁 Volver a Documentación](./README.md)

# 🚀 Documentación de Endpoints (MVP)

A continuación se documentan los métodos HTTP requeridos para las pantallas principales de Vitapet, basándonos en el estándar REST y Swagger.

### 1. Pantalla de Registro de Usuario (`Register.tsx`)
* **Método:** `POST`
* **Ruta sugerida:** `/api/users/register`
* **Descripción:** Se utiliza el método POST porque el cliente (interfaz) está enviando información sensible y nueva (nombre, email y contraseña) al servidor para crear un recurso nuevo en la base de datos (un usuario).
* **Payload de ejemplo:** [registro_usuario.json](./registro_usuario.json)

### 2. Pantalla de Perfil de Mascota (`PetProfile.tsx`)
Esta pantalla requiere dos operaciones distintas:

* **Método:** `GET`
    * **Ruta sugerida:** `/api/pets/{id}`
    * **Descripción:** Se utiliza el método GET al cargar la pantalla para consultar y obtener toda la información de la mascota (nombre, vacunas, historial de peso) sin modificar nada en el servidor.
    
* **Método:** `POST`
    * **Ruta sugerida:** `/api/pets/{id}/weight`
    * **Descripción:** Al registrar un nuevo peso en la cartilla, se utiliza POST para enviar el nuevo registro (peso y fecha) y añadirlo al historial de la mascota en la base de datos.
* **Payload de ejemplo:** [registro_peso.json](./registro_peso.json)
