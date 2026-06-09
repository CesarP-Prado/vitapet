[⬅️ Volver al Inicio](../README.md)

# 📚 Documentación Técnica de Vitapet

Esta carpeta centraliza todos los documentos, diagramas, esquemas de datos (payloads) y notas técnicas necesarias para el desarrollo de Vitapet.

## 🗂️ Índice de Archivos

- [Historias de Usuario](./historias_de_usuarios.md): Detalle de las historias de usuario y sus criterios de aceptación para el MVP.
- [Identificación de Campos](./identificacion_de_campos.md): Mapeo de los campos requeridos en la interfaz según el prototipo de Figma.
- [Referencia de API (Endpoints)](./endpoints.md): Documentación de las rutas, métodos HTTP y payloads de la aplicación.
- [Payload: Registro de Usuario](./registro_usuario.json): Estructura JSON enviada al registrar una nueva cuenta.
- [Payload: Registro de Peso](./registro_peso.json): Estructura JSON enviada al registrar un nuevo pesaje de la mascota.

---

## 📖 Historias de Usuario Principales (Resumen)

**1️⃣ US-01 — Alertas de Medicación**
> *Como dueño, quiero recibir recordatorios exactos de medicación para no olvidar la dosis de mi mascota.*

- **Flujo de éxito:** Hora programada → Notificación push → Abre app → Ve tarea en Home → Confirma dosis → Registrado en historial ✅
- **Alternativo:** Usuario no abre la app → Re-recordatorio en 15 min → reintenta

**2️⃣ US-02 — Registrar Consulta Médica**
> *Como dueño, quiero registrar una consulta veterinaria para mantener el historial clínico actualizado.*

- **Flujo de éxito:** Home → Tab Mascotas → Historial Clínico → Toca "+" → Llena formulario → Consulta guardada ✅
- **Alternativo:** Formulario incompleto → Alerta de error en rojo → Regresa a corregir

> 💡 *Para ver el detalle completo con todos los criterios de aceptación, revisa el archivo de [Historias de Usuario](./historias_de_usuarios.md).*

---

## 📝 Resumen de Campos de Interfaz (MVP)

A continuación se resumen los campos de captura de información requeridos por cada módulo principal, extraídos del diseño del prototipo:

- **Login / Registro:** Nombre Completo, Correo, Contraseña.
- **Registro de Mascota:** Nombre, Especie, Raza, Fecha de Nacimiento.
- **Medicación:** Mascota a medicar, Nombre del medicamento, Dosis, Frecuencia, Fecha de inicio, Hora.
- **Higiene:** Mascota, Actividad, Tipo, Última vez, Próxima vez.
- **Perfil (Cartilla de Peso):** Peso en kg.

> 💡 *Para ver el detalle técnico completo y los tipos de dato de cada campo, revisa el archivo de [Identificación de Campos](./identificacion_de_campos.md).*

---

## 🚀 Documentación de Endpoints (MVP)

Actualmente, la arquitectura backend del MVP de Vitapet cuenta con rutas esenciales para los flujos de autenticación de usuario y registro clínico de la mascota. Dado que el prototipo incluye pantallas de medicación y control de higiene, esta lista se irá expandiendo.

> 💡 *Para revisar las rutas exactas, métodos HTTP (`GET`, `POST`, etc.) y esquemas JSON requeridos en las peticiones, consulta la **[Referencia Completa de API (Endpoints)](./endpoints.md)**.*
