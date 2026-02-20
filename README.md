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
