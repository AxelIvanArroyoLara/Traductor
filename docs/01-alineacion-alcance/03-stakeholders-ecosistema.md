# Stakeholders y Ecosistema — Fase 1

## Estado
Borrador estratégico consolidado

## Owner
T2 — Bruno (Tech Lead / Sistemas)

## Objetivo

Consolidar en un solo documento el análisis estratégico del producto SaaS de traducción asistida por IA en Fase 1, integrando:

- Identificación de stakeholders.
- Tensiones estratégicas.
- Estructura operativa del ecosistema.
- Dependencias técnicas críticas.
- Implicaciones para arquitectura y modelo de dominio.

---

# 1. Contexto del Producto (Fase 1)

El producto se plantea como un **SaaS enfocado inicialmente en traductores profesionales y trabajadores de idiomas**, con las siguientes características diferenciadoras:

- Traducción asistida por IA contextual.
- Personalización por proyecto o cliente.
- Enfoque en confidencialidad y seguridad.
- No sustitución del traductor, sino asistencia.

El modelo de IA aún está en fase de definición (propio, open-source o externo).

---

# 2. Mapa de Stakeholders (Enfoque Estratégico)

El mapa de stakeholders identifica los actores que influyen o son influenciados por el sistema, así como las tensiones que generan.

## 2.1 Stakeholder Central (Core Audience)

### Traductor profesional / freelance / profesor-traductor

Actor principal del sistema.

Intereses:

- Velocidad.
- Calidad contextual.
- Confidencialidad.
- Control sobre su información.
- Propiedad de datos.
- Personalización por cliente.

Define:

- Requisitos funcionales.
- UX.
- Modelo de dominio inicial.
- Propuesta de valor.

---

## 2.2 Stakeholders Internos

### Equipo de desarrollo

Impacta directamente:

- Arquitectura.
- Seguridad real.
- Escalabilidad.
- Desacoplamiento del modelo IA.

---

### Estudiantes y profesores de idiomas

Segmento secundario en Fase 1, pero relevante para:

- Casos de uso educativos.
- Posible expansión futura.

---

## 2.3 Stakeholders Externos

### Clientes corporativos del traductor

Empresas, despachos, editoriales o instituciones que generan los documentos.

Influyen en:

- Requisitos de confidencialidad.
- Persistencia o eliminación de datos.
- Necesidad de gestión por proyecto.
- Contextualización técnica.

---

### Competidores

Ejemplo: DeepL y otras plataformas de traducción asistida.

Generan presión en:

- Estándares de calidad.
- Velocidad.
- Precio.
- Simplicidad.

---

### Proveedores tecnológicos

Incluyen:

- Hosting.
- Base de datos.
- Servicios de cifrado.
- Posible proveedor de modelo IA.

Impactan:

- Costos.
- Disponibilidad.
- Latencia.
- Seguridad efectiva.

---

### Reguladores de protección de datos

Condicionan:

- Manejo de datos.
- Retención.
- Eliminación segura.
- Logs y auditoría.

---

# 3. Tensiones Estratégicas Identificadas

## 3.1 Velocidad vs Seguridad

El usuario desea rapidez.  
El sistema promete confidencialidad.

Impacta decisiones en:

- Persistencia.
- Cifrado.
- Procesamiento del modelo.

---

## 3.2 Personalización vs Escalabilidad

Diferenciador:

- Glosarios.
- Memoria contextual.
- Proyectos por cliente.

Implica:

- Modelo de dominio complejo.
- Separación multi-tenant.
- Diseño modular.

---

## 3.3 Diferenciación vs Dependencia del Modelo IA

Si el modelo es externo:

- Existe dependencia técnica.
- Riesgo de costos variables.
- Riesgo de cambios de licencia.

Esto convierte al proveedor de modelo en stakeholder crítico.

---

# 4. Mapa de Ecosistema (Enfoque Operacional)

El mapa de ecosistema traduce las tensiones estratégicas en estructura operativa.

Responde a:

- Cómo fluye la información.
- Cómo fluye el dinero.
- Cómo fluye la dependencia técnica.

---

## 4.1 Límite del Sistema

Sistema central:

> Plataforma SaaS de traducción asistida por IA.

Incluye:

- Gestión de usuarios.
- Gestión de proyectos.
- Integración con modelo IA.
- Seguridad.
- Control de acceso.
- Persistencia de datos (según política).

---

## 4.2 Actores del Ecosistema y Flujos

### Traductor

Flujo de información:

Traductor → Plataforma → Modelo IA → Plataforma → Traductor

Flujo económico:

Traductor → Suscripción → Plataforma

---

### Clientes del Traductor

Clientes → Traductor → Plataforma

Generan:

- Documentos.
- Contexto.
- Requisitos de seguridad.

---

### Plataforma SaaS

Orquesta:

- Autenticación.
- RBAC.
- Cifrado.
- Separación multi-tenant.
- Comunicación con modelo IA.

Es el núcleo estructural.

---

### Modelo IA

Flujo técnico:

Plataforma → texto  
Modelo → sugerencia

Debe diseñarse como módulo desacoplado.

---

### Infraestructura tecnológica

Sostiene:

- Servidores.
- Base de datos.
- Almacenamiento.
- Seguridad.
- Red.

Impacta escalabilidad y costos.

---

### Pasarela de pagos (si aplica)

Traductor → Pago → Plataforma

Impacta:

- Planes.
- Restricción por uso.
- Control de acceso premium.

---

# 5. Diferencia entre Stakeholders y Ecosistema

Stakeholders:
- Analiza actores y presiones estratégicas.

Ecosistema:
- Analiza estructura operativa y dependencias técnicas.

Ambos son complementarios:

Stakeholders → Qué fuerzas afectan el sistema.  
Ecosistema → Cómo el sistema funciona dentro de esas fuerzas.

---

# 6. Implicaciones para Fase 1

Dado que el producto inicia como SaaS individual:

- Multi-tenancy es obligatorio.
- Separación lógica por usuario es crítica.
- El modelo IA debe abstraerse.
- Seguridad es diferenciador competitivo.
- La arquitectura debe anticipar expansión a cuentas organizacionales.

Este análisis impacta directamente:

- Modelo de dominio (Doc 09).
- RBAC (Doc 10).
- Reglas y validaciones (Doc 15).
- Arquitectura lógica.

---

# 7. Referencias

- Brief de producto.
- Backlog priorizado.
- Decisiones pendientes sobre modelo IA.
