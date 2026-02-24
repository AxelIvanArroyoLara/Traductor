# Backlog de Requisitos y Registro de Decisiones

## 1. Introducción
Este documento contiene el backlog de requisitos y el registro de decisiones del proyecto correspondiente a la Fase 1, priorizando la seguridad y confidencialidad de la información.

## 2. Objetivo
Definir requisitos, priorizar funcionalidades, registrar decisiones y garantizar el manejo seguro de archivos confidenciales.

## 3. Metodología de Priorización (MoSCoW)

| Nivel | Descripción |
|-------|-------------|
| Must | Requisito obligatorio |
| Should | Requisito importante |
| Could | Requisito deseable |
| Won’t | Fuera del alcance actual |

## 4. Requisitos Funcionales

| ID | Descripción | Prioridad | Criterio | Estado |
|----|-------------|-----------|----------|--------|
| RF-01 | Inicio de sesión con Google | Must | Cuenta válida | Pendiente |
| RF-02 | Control de acceso | Must | Autenticado | Pendiente |
| RF-03 | Gestión de usuarios | Should | CRUD | Pendiente |
| RF-04 | Almacenamiento local | Must | BD local | Pendiente |
| RF-05 | Consulta de archivos | Should | Búsqueda | Pendiente |

## 5. Requisitos No Funcionales

| ID | Requisito | Prioridad | Estado |
|----|-----------|-----------|--------|
| RNF-01 | Seguridad | Must | Pendiente |
| RNF-02 | Privacidad | Must | Pendiente |
| RNF-03 | Rendimiento | Should | Pendiente |
| RNF-04 | Disponibilidad local | Must | Pendiente |

## 6. Reglas de Negocio

| ID | Regla | Impacto |
|----|-------|---------|
| RB-01 | Autenticación obligatoria con Google | Alto |
| RB-02 | Prohibido uso de nube | Alto |
| RB-03 | Almacenamiento solo local | Alto |
| RB-04 | Protección de archivos confidenciales | Alto |
| RB-05 | Cierre automático de sesión | Medio |

## 7. Registro de Decisiones

| No. | Decisión | Justificación | Estado |
|-----|----------|--------------|--------|
| 1 | Base de datos local sencilla | Mayor control y privacidad | Aprobada |
| 2 | Login con Google | Seguridad y simplicidad | Aprobada |
| 3 | No uso de servicios cloud | Protección de información | Aprobada |

## 8. Riesgos

| Riesgo | Impacto | Mitigación |
|--------|----------|------------|
| Filtración de datos | Alto | Controles de acceso |
| Fallas en BD local | Medio | Respaldos |
| Errores humanos | Medio | Buen diseño de interfaz |

## 9. Conclusión
El presente documento establece una base sólida para el desarrollo del sistema, priorizando la seguridad, confidencialidad y control local de la información.
