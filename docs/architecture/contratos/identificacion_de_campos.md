[⬅️ Volver al Inicio](../README.md) | [📁 Volver a Documentación](./README.md)

# Escaneo de Figma - MVP Vitapet

A continuación se listan los campos de información requeridos para todas las pantallas clave del MVP, extraídos directamente del prototipo.

## Pantalla 1: Login (`Login.tsx`)
* **Campo de correo:** `Correo Electrónico` (Tipo: String / Email)
* **Campo de contraseña:** `Contraseña` (Tipo: String / Password)

## Pantalla 2: Registro de Cuenta (`Register.tsx`)
* **Campo de texto:** `Nombre Completo` (Tipo: String)
* **Campo de correo:** `Correo Electrónico` (Tipo: String / Email)
* **Campo de contraseña:** `Contraseña` (Tipo: String / Password)

## Pantalla 3: Lista y Registro de Mascotas (`PetsList.tsx`)
* **Campo de texto:** `Nombre` (Tipo: String)
* **Selector:** `Especie` (Tipo: String/Enum - ej. Perro, Gato)
* **Campo de texto (Opcional):** `Raza` (Tipo: String)
* **Campo de fecha:** `Fecha de Nacimiento` (Tipo: Date)

## Pantalla 4: Perfil de Mascota - Agregar Peso (`PetProfile.tsx` / `Profile.tsx`)
* **Identificador oculto:** `ID de Mascota` (Tipo: String / UUID extraído de la URL)
* **Campo numérico:** `Peso en kg` (Tipo: Float / Decimal)
* **Dato de sistema:** `Fecha actual` (Tipo: Date / ISO String - se genera automáticamente al guardar)

## Pantalla 5: Módulo de Medicación (`Medication.tsx`)
* **Selector:** `Mascota` (Tipo: String / UUID de la mascota)
* **Campo de texto:** `Nombre del medicamento` (Tipo: String)
* **Campo de texto:** `Dosis` (Tipo: String)
* **Campo de texto:** `Frecuencia` (Tipo: String)
* **Campo de fecha:** `Fecha de inicio` (Tipo: Date)
* **Campo de tiempo:** `Hora` (Tipo: Time / String)

## Pantalla 6: Agenda de Higiene (`Hygiene.tsx`)
* **Selector:** `Mascota` (Tipo: String / UUID de la mascota)
* **Campo de texto:** `Actividad` (Tipo: String - ej. Baño general)
* **Selector:** `Tipo` (Tipo: String/Enum)
* **Campo de fecha (Opcional):** `Última vez` (Tipo: Date)
* **Campo de fecha:** `Próxima vez` (Tipo: Date)

## Pantalla 7: Dashboard (`Dashboard.tsx`)
* *Esta pantalla es de solo lectura (visualización de alertas y tareas del día), no requiere campos de entrada manual por parte del usuario.*