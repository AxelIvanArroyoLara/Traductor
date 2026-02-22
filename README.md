# Diseño de Producto — Fase 1

## Objetivo
Repositorio de entregables de diseño para Fase 1 (alcance, investigación, arquitectura, flujos, validación y UI final).

## Stack de trabajo
- **Docs:** Markdown en GitHub
- **Diagramas:** draw.io / diagrams.net
- **UI y prototipo:** Figma
- **Seguimiento:** GitHub Issues + GitHub Projects

## Equipo
- **U1 — UX Research / Producto (Dani):** Lidera investigación con usuarios, síntesis de insights, definición de necesidades/JTBD, validación de flujos desde negocio/usuario y plan de pruebas de usabilidad.
- **U2 — UI/UX Design (Naia):** Lidera arquitectura visual y experiencia de interfaz: wireframes, diseño UI de alta fidelidad, prototipo navegable, componentes/UI kit y documentación visual para handoff.
- **T1 — Product/Tech Analyst (Mike):** Traduce necesidades de producto a requisitos funcionales y reglas; lidera backlog, criterios de éxito, RBAC, casos de uso, reglas/validaciones y consistencia funcional entre diseño y desarrollo.
- **T2 — Tech Lead / Sistemas (Bruno):** Lidera definición técnica del sistema: arquitectura lógica, modelo de dominio, procesos complejos (BPMN/estados), restricciones técnicas, integraciones y viabilidad de implementación.
- **PM — Project Manager (Iván):** Coordina el plan de trabajo diario, prioridades, seguimiento en GitHub (Issues/Project), gestión de bloqueos, alineación con stakeholders y control de tiempos/entregables. Proporciona apoyo directo en todas las áreas del proyecto.

# Tabla RACI por entregable y día (2 semanas / 10 días hábiles)

## Roles
- **U1** = UX Research / Producto
- **U2** = UI/UX Design
- **T1** = Product/Tech Analyst
- **T2** = Tech Lead / Sistemas

## Leyenda RACI
- **R** = Responsable (ejecuta)
- **A** = Accountable (dueño final / quien cierra)
- **C** = Consultado
- **I** = Informado

| Día | Entregable | Owner | U1 | U2 | T1 | T2 |
|---|---|---|---|---|---|---|
| 1 | **1. Brief de producto (1-pager)** | U1 | A/R | C | C | I |
| 1 | **2. Backlog de requisitos priorizado + registro de decisiones** | T1 | C | I | A/R | C |
| 1 | **3. Mapa de stakeholders y ecosistema** | T2 | C | I | C | A/R |
| 2 | **4. Plan y guía de entrevistas** | U1 | A/R | R | C | C |
| 3–4 | **5. Síntesis de entrevistas** | U1 | A/R | R | C | I |
| 3–4 | **6. Personas / perfiles (fase 1 + anexos F2)** | U2 | C | A/R | I | I |
| 4 | **7. Jobs-to-be-done / Casos de uso** | T1 | C | I | A/R | C |
| 5 | **8. Sitemap / arquitectura de información** | U2 | R | A/R | C | C |
| 5 | **9. Modelo de dominio (entidades y relaciones)** | T2 | I | I | C | A/R |
| 5 | **10. Matriz de roles y permisos (RBAC)** | T1 | I | I | A/R | C |
| 5 | **11. (Opcional) Matriz de funcionalidades por plan** | T1 | I | C | A/R | C |
| 6 | **12. User flows por objetivo (fase 1)** | U1 | A/R | R | C | C |
| 7 | **13. Diagramas de actividad / BPMN (procesos complejos)** | T1 | C | I | A/R | R |
| 7 | **14. Diagramas de estados (state machine)** | T2 | I | I | C | A/R |
| 6–7 | **15. Especificación de reglas y validaciones** | T1 | C | C | A/R | R |
| 8 | **16. Plan de pruebas de usabilidad + guión** | U1 | A/R | R | C | I |
| 9 | **17. Reporte de testing** | T1 | R | C | A/R | C |
| 10 | **18. Diseño de UI completo (alta fidelidad)** | U2 | C | A/R | R | R |

---

## Nota operativa
- **Equipo usuario/diseño (U1, U2):** lidera 4, 5, 6, 8, 12, 16, 18 (y co-lidera validación de 17)
- **Equipo técnico (T1, T2):** lidera 2, 3, 9, 10, 11, 13, 14, 15
- **Dependencias críticas:** 1–3 → 4–7 → 8–15 → 16–17 → 18
## Entregables
### 1) Alineación y alcance
- [01. Brief de producto](docs/01-alineacion-alcance/01-brief-producto.md)
- [02. Backlog + decisiones](docs/01-alineacion-alcance/02-backlog-requisitos-y-decisiones.md)
- [03. Stakeholders y ecosistema](docs/01-alineacion-alcance/03-stakeholders-ecosistema.md)

### 2) Investigación y usuarios
- [04. Plan y guía de entrevistas](docs/02-investigacion-usuarios/04-plan-guia-entrevistas.md)
- [05. Síntesis de entrevistas](docs/02-investigacion-usuarios/05-sintesis-entrevistas.md)
- [06. Personas / perfiles](docs/02-investigacion-usuarios/06-personas-perfiles.md)
- [07. JTBD / Casos de uso](docs/02-investigacion-usuarios/07-jtbd-casos-de-uso.md)

### 3) Arquitectura y estructura
- [08. Sitemap / IA](docs/03-arquitectura-producto/08-sitemap-arquitectura-informacion.md)
- [09. Modelo de dominio](docs/03-arquitectura-producto/09-modelo-dominio.md)
- [10. RBAC](docs/03-arquitectura-producto/10-rbac-roles-permisos.md)
- [11. Funcionalidades por plan (opcional)](docs/03-arquitectura-producto/11-funcionalidades-por-plan.md)

### 4) Flujos, lógica y procesos
- [12. User flows](docs/04-flujos-logica-procesos/12-user-flows.md)
- [13. BPMN](docs/04-flujos-logica-procesos/13-bpmn-procesos.md)
- [14. Diagramas de estados](docs/04-flujos-logica-procesos/14-diagramas-estados.md)
- [15. Reglas y validaciones](docs/04-flujos-logica-procesos/15-reglas-validaciones.md)

### 5) Validación
- [16. Plan de pruebas](docs/05-validacion/16-plan-pruebas-usabilidad.md)
- [17. Reporte de testing](docs/05-validacion/17-reporte-testing.md)

### 6) UI final
- [18. Diseño UI completo](docs/06-ui-final/18-diseno-ui-completo.md)

## Gestión
- [RACI](project-management/raci.md)
- [Registro diario](project-management/daily-log/)
- [ADRs / Decisiones](project-management/decisions/)
- [Links de Figma](ui/figma-links.md)
