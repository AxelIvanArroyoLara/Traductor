# Reporte de Testing — Sistema Traductor

## Estado
Pendiente

## Owner
T1 — Product/Tech Analyst

## Objetivo
Este documento describe las **pruebas realizadas** en el sistema **Traductor**, con el propósito de verificar que las funcionalidades implementadas cumplen con los requisitos establecidos y se comportan como se espera en los diferentes escenarios de uso.

---

## 1. Resumen de las pruebas

**Fecha de ejecución**: Pendiente  
**Versión del sistema**: Pendiente  
**Entorno de pruebas**: Local (sin nube)

---

## 2. Tipos de pruebas

Las pruebas realizadas abarcan los siguientes tipos:

- **Pruebas de integración**: Verificación de que los módulos del sistema interactúan correctamente.
- **Pruebas de interfaz de usuario (UI)**: Asegurarse de que los elementos visibles y las interacciones con la interfaz de usuario sean correctas.
- **Pruebas de validaciones**: Verificación de que los datos y entradas sean correctos y se validen apropiadamente.
- **Pruebas de reglas de negocio**: Validación de las reglas funcionales del sistema.
- **Pruebas de rendimiento**: Evaluación del rendimiento del sistema bajo carga (carga de archivos, traducción de documentos, etc.).

---

## 3. Casos de prueba

A continuación se presentan los **casos de prueba** que serán ejecutados, organizados por **funcionalidad**.

### 3.1 Iniciar sesión

| ID | Caso de prueba | Resultado esperado | Resultado actual | Estado |
|---|---|---|---|---|
| CP-01 | Iniciar sesión con Google | El sistema debe permitir iniciar sesión con Google | Pendiente | Pendiente |
| CP-02 | Validación de sesión expirada | El sistema debe redirigir a login si la sesión expira | Pendiente | Pendiente |
| CP-03 | Intentar login sin credenciales | El sistema debe mostrar un error si no se ingresan credenciales | Pendiente | Pendiente |

---

### 3.2 Gestión de documentos

| ID | Caso de prueba | Resultado esperado | Resultado actual | Estado |
|---|---|---|---|---|
| CP-04 | Importar archivo compatible | El sistema debe permitir importar documentos PDF, DOCX, TXT | Pendiente | Pendiente |
| CP-05 | Importar archivo no compatible | El sistema debe bloquear la importación y mostrar un mensaje | Pendiente | Pendiente |
| CP-06 | Crear documento | El sistema debe permitir crear un documento desde la interfaz | Pendiente | Pendiente |
| CP-07 | Eliminar documento | El sistema debe requerir confirmación antes de eliminar un documento | Pendiente | Pendiente |

---

### 3.3 Traducción

| ID | Caso de prueba | Resultado esperado | Resultado actual | Estado |
|---|---|---|---|---|
| CP-08 | Selección de idioma | El sistema debe permitir seleccionar un idioma de origen y destino | Pendiente | Pendiente |
| CP-09 | Iniciar traducción sin seleccionar idioma | El sistema debe bloquear el botón de "Iniciar traducción" hasta seleccionar idioma | Pendiente | Pendiente |
| CP-10 | Traducir documento | El sistema debe permitir la traducción de un documento después de elegir el idioma | Pendiente | Pendiente |
| CP-11 | Cancelar traducción | El sistema debe permitir cancelar una traducción en cola o en ejecución | Pendiente | Pendiente |

---

### 3.4 Glosarios

| ID | Caso de prueba | Resultado esperado | Resultado actual | Estado |
|---|---|---|---|---|
| CP-12 | Crear glosario | El sistema debe permitir crear un glosario por proyecto | Pendiente | Pendiente |
| CP-13 | Editar glosario | El sistema debe permitir editar un glosario existente | Pendiente | Pendiente |

---

## 4. Validaciones realizadas

### 4.1 Iniciar sesión

| ID | Validación | Dónde | Regla asociada | Si falla | Mensaje sugerido |
|---|---|---|---|---|---|
| VAL-01 | Campos de inicio de sesión | UI | RB-01 | Bloqueante | "Por favor, ingresa tus credenciales para continuar." |
| VAL-02 | Sesión válida | Local | RB-02 | Bloqueante | "Tu sesión ha expirado, por favor inicia sesión nuevamente." |

### 4.2 Importar documento

| ID | Validación | Dónde | Regla asociada | Si falla | Mensaje sugerido |
|---|---|---|---|---|---|
| VAL-10 | Tipo de archivo soportado | UI/Local | RB-04 | Bloqueante | "El archivo debe ser un PDF, DOCX o TXT." |
| VAL-11 | Tamaño máximo de archivo | Local | RB-04 | Bloqueante | "El archivo excede el tamaño máximo permitido." |
| VAL-12 | Documento cargado | Local | RB-05 | Bloqueante | "Debes asignar el documento a un proyecto antes de cargarlo." |

### 4.3 Traducción

| ID | Validación | Dónde | Regla asociada | Si falla | Mensaje sugerido |
|---|---|---|---|---|---|
| VAL-20 | Idioma seleccionado | UI | RB-08 | Bloqueante | "El idioma de origen y destino deben estar seleccionados antes de traducir." |
| VAL-21 | Estado de traducción | Local | RB-09 | Bloqueante | "El sistema debe mostrar el estado de traducción: 'en cola', 'ejecutándose', 'terminado' o 'fallido'." |

---

## 5. Resultados de las pruebas de rendimiento

### 5.1 Importación de archivos

| ID | Caso de prueba | Descripción | Resultado |
|---|---|---|---|
| PR-01 | Importar archivo grande (10MB) | Evaluar el tiempo de respuesta al importar un archivo grande | Pendiente |

### 5.2 Traducción de documentos

| ID | Caso de prueba | Descripción | Resultado |
|---|---|---|---|
| PR-02 | Traducir documento de 10,000 palabras | Evaluar el tiempo que tarda en traducir un documento grande | Pendiente |

---

## 6. Conclusiones

- **Funcionalidad completa**: Aún pendiente de realizar las pruebas completas.
- **Reglas y validaciones**: Las reglas de negocio y validaciones se están implementando correctamente.
- **Rendimiento**: Aún no se ha probado completamente el rendimiento.



---

**Fecha de ejecución**: Pendiente  
**Versión del sistema**: Pendiente  
**Entorno de pruebas**: Local (sin nube)
