# Entregables (Fase de diseño)

### 1) Alineación y alcance

1. **Brief de producto (1-pager)**

   * Objetivo, alcance Fase 1 vs Fase 2 (alumnado marcado como F2), KPIs, supuestos, riesgos, stakeholders.

2. **Backlog de requisitos priorizado + registro de decisiones**

   * MoSCoW/RICE, dependencias, “decidido / pendiente”, y criterios de éxito por bloque.

3. **Mapa de stakeholders y ecosistema**

   * Actores, responsabilidades, dependencias, integraciones externas y límites del sistema.

---

### 2) Investigación y definición de usuarios

4. **Plan y guía de entrevistas**

   * Guiones por tipo de usuario y objetivos de aprendizaje.

5. **Síntesis de entrevistas**

   * Insights, pains/gains, oportunidades, y matriz de hallazgos.

6. **Personas / perfiles (fase 1 + anexos F2)**

   * 2–4 para fase 1; perfiles de alumnado sólo como referencia futura (F2).

7. **Jobs-to-be-done / Casos de uso**

   * Necesidades por rol + métricas de éxito.

---

### 3) Arquitectura y estructura del producto

8. **Sitemap / arquitectura de información**

   * Módulos, navegación, jerarquía, secciones y rutas principales.

9. **Modelo de dominio (entidades y relaciones)**

   * Objetos clave, relaciones, atributos críticos (sirve para no “inventar” cosas en UI).

10. **Matriz de roles y permisos (RBAC)**

* Rol → acción → módulo (incluye restricciones y casos borde).

11. **(Opcional) Matriz de funcionalidades por plan**

* Si habrá tiers, límites y disponibilidad por plan.

---

### 4) Flujos, lógica y procesos

12. **User flows por objetivo (fase 1)**

* Happy path + alternos + errores; lo de F2 se etiqueta y se manda a anexo.

13. **Diagramas de actividad / BPMN (procesos complejos)**

* Para reglas, aprobaciones, handoffs, y pasos con excepciones.

14. **Diagramas de estados (state machine)**

* Para objetos con ciclo de vida (borrador → en proceso → finalizado → fallido → reintento, etc.).

15. **Especificación de reglas y validaciones**

* Reglas de negocio, límites, mensajes, manejo de errores, reintentos, timeouts.

---

### 5) Validación

16. **Plan de pruebas de usabilidad + guión**

* Tareas, muestra, criterios, métricas (éxito, tiempo, fricción).

17. **Reporte de testing**

* Hallazgos priorizados + cambios propuestos + decisiones.

---

## 6) Entrega final única: Diseño UI (incluye TODO lo visual + wireframes)

18. **Diseño de UI completo (alta fidelidad)**

* **Wireframes + UI final + prototipo navegable** (todo dentro del mismo entregable)
* Pantallas de todos los módulos de fase 1
* Estados completos: vacío / loading / error / success
* Componentes reutilizables (UI kit básico) + tokens (tipografía, color, spacing)
* Especificación de interacción (hover, focus, modales, validaciones)
* Hand-off para desarrollo (medidas, componentes, comportamiento)

---

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

---
