# Vitapet — Diseño UX/UI

**Proyecto:** Vitapet — App móvil de gestión de salud y bienestar para mascotas  
**Equipo:** Jahaziel Barajas, Cesar Prado  
**Asignatura:** Administración de Proyectos de Software  
**Profesor:** José Alfredo Martínez Cosío  
**Institución:** CESUN Universidad  
**Grupo:** 07IDESVA | Cuatrimestre: Séptimo | 2026

---

## Enlace de Figma (Modo Presentación)

> 🔗 **[Ver prototipo interactivo en Figma](https://www.figma.com/team_invite/redeem/jrTj5zcc62Jx7jjI28WFgj?t=Gx4kPE8N5yEYnSxi-21)**
>
> El prototipo incluye las pantallas conectadas de forma interactiva para calificación en modo Presentación.

---

## Archivos en esta carpeta

| Archivo | Descripción |
|---|---|
| `sitemap.png` | Mapa de todas las pantallas del MVP de Vitapet |
| `user_flows.pdf` | Diagramas de flujo de las 2 historias de usuario principales |
| `README.md` | Este archivo — contiene el enlace de Figma |

---

## Pantallas diseñadas

### Pantalla 1 — Login / Registro
- Formulario de email + contraseña
- Autenticación con Google (OAuth)
- Enlace a registro de nueva cuenta
- Logo y tagline de Vitapet

### Pantalla 2 — Home / Dashboard
- Tarjeta de mascota activa con estatus de salud
- Lista de tareas del día (medicación, higiene, vacunas)
- Estados visuales: urgente / normal / completado
- Navegación inferior con 4 tabs

### Pantalla 3 — Historial Clínico (función principal)
- Tabs: Consultas / Vacunas / Peso
- Tarjetas de visita con indicador de color por estado
- Botón para agregar nueva entrada
- Detalle completo de cada consulta

---

## Historias de Usuario principales

**US-01 — Alertas de Medicación**
> Como dueño, quiero recibir recordatorios exactos de medicación para no olvidar la dosis de mi mascota.

**Flujo de éxito:** Hora programada → Notificación push → Abre app → Ve tarea en Home → Confirma dosis → Registrado en historial ✅

**Flujo alternativo (No):** Usuario no abre la app → Re-recordatorio en 15 min → reintenta

---

**US-02 — Registrar Consulta Médica**
> Como dueño, quiero registrar una consulta veterinaria para mantener el historial clínico de mi mascota actualizado.

**Flujo de éxito:** Home → Tab Mascotas → Historial Clínico → Toca "+" → Llena formulario → Campos completos → Consulta guardada ✅

**Flujo alternativo (No):** Formulario incompleto → Alerta de error en rojo → Regresa a corregir

---

## Repositorio GitHub

🔗 [https://github.com/CesarP-Prado/vitapet](https://github.com/CesarP-Prado/vitapet)

---

## Estilo de diseño

El diseño sigue un estilo **minimalista y limpio** inspirado en apps de salud y bienestar modernas, con:
- Paleta de colores: azul principal, verde para estados saludables, ámbar para alertas, rojo para urgente
- Tipografía clara y legible en móvil
- Navegación bottom tab bar con 4 secciones principales
- Cards con indicadores de color para estados de salud

---

*Última actualización: Junio 2026*
