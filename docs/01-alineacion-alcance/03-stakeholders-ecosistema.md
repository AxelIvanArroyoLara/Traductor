# Stakeholders y Ecosistema — Fase 1

## Estado
Borrador estratégico consolidado

## Owner
T2 — Bruno (Tech Lead / Sistemas)

## Objetivo

Consolidar en un solo documento el análisis estratégico del producto SaaS de traducción asistida por IA en Fase 1, integrando los siguientes aspectos:

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
- No sustitución del traductor, sino asistencia para la traducción de documentos largos y complejos.

En estos momentos el modelo de IA se encuentra aún en fase de definición (ya sea propio, open-source o externo).

---

# 2. Mapa de Stakeholders (Enfoque Estratégico)

El mapa de stakeholders identifica los actores que influyen o son influenciados por el sistema, así como las tensiones que generan.

![Mapa de Stakeholders](../../diagrams/stakeholders-y-ecosistema/WS-Stakeholders-Traductor.png)

## 2.1 Stakeholder Central (Core Audience)

### Traductor profesional / freelance / profesor-traductor

Es el actor principal del sistema. Cuenta con los siguientes **intereses**:

- Velocidad.
- Calidad contextual.
- Confidencialidad.
- Control sobre su información.
- Propiedad de datos.
- Personalización por cliente.

Por los anteriores criterios, define e influye en:

- Requisitos funcionales.
- UX.
- Modelo de dominio inicial.
- Propuesta de valor.

En resumen, es el cliente y en quien va a recaer el diseño del producto. Es vital mantenerlo cerca por si existe la presencia de nuevos intereses.

---

## 2.2 Stakeholders Internos

### Equipo de desarrollo

En este caso, WolfDevelopment Studios. Impactan directamente en:

- Arquitectura del producto.
- Seguridad real.
- Escalabilidad.
- Desacoplamiento del modelo IA.

---

### Estudiantes y profesores de idiomas

Son un segmento secundario en Fase 1 ya que el objetivo clave son los traductos, no obstante son relevantes para:

- Casos de uso educativos.
- Posible expansión futura.

Con respecto a esto úlitmo, al ser uno de los clientes "profesor-traductor", los estudiante y profesores de idiomas son un grupo al que influenciaran tarde o temprano en el desarrollo.

---

## 2.3 Stakeholders Externos

### Clientes corporativos del traductor

A clientes coorporativos se consideran: Empresas, despachos, editoriales o instituciones que generan los documentos. Son aquellos que envían la información al traductor y tienen especial énfasis en la seguridad de la manipulación de datos.

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
- **Precio**.
- Simplicidad.

---

### Proveedores tecnológicos

A proveedores tecnológicos incluyo a proveedores existentes de: Hosting, base de datos, servicios de cifrado, y posible proveedor de modelo IA.

Los provedores impactan en:

- Costos.
- Disponibilidad.
- Latencia.
- Seguridad efectiva.

Los proveedores definen estándares de **seguridad y experiencias** para los usuarios.

---

### Reguladores de protección de datos

Condicionan:

- Manejo de datos.
- Retención.
- Eliminación segura.
- Logs y auditoría.

De igual forma, estén presentes al momento en que el los clientes comprueban el uso de IA en documentos del traductor.

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
- No verificable por verificadores de IA.

Implica:

- Modelo de dominio complejo.
- Separación multi-tenant.
- Diseño modular.
- Humanización de texto.

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

![Mapa de Stakeholders](../../diagrams/stakeholders-y-ecosistema/Diagrama-de-Ecosistema-WS-Traductor.png)

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

#### Flujo de información del traductor:
Para el flujo de información hay que considerar que en primer lugar, el traductor recibe un documento de parte de su cliente y este documento debe de ser traducido a otro idioma. Para tal documento, el traductor accede a la plataforma, lo sube y selecciona, la plataforma envía el texto a procesar al modelo de IA. El modelo de IA ahora envía las segurencias a la plataforma; la plataforma por su parte ofrece las sugerencias, alternativas glosarios y contexto al traductor para realizar el trabajo. Finalmente, el traductor envía la información a su cliente.

Lo anterior se presenta tal que: 
Cliente → Traductor → Plataforma → Modelo IA → Plataforma → Traductor → Cliente

#### Flujo económico:
El flujo de pago se puede simplificar de la siguietne forma:

Traductor → Pasarela de pago → Plataforma

---

### Clientes del Traductor
#### Flujo de información
Para el caso de los clientes, estos envían el documento al traductor, el traductor sigue su flujo de información y cuando recibe la entrega final, verifica con los reguladores que se cumplan todos los requirimientos necesarios y comprueba que los detectores de IA no muestren resultados preocupantes.
Clientes → Traductor → Plataforma → Traductor → Clientes → Reguladores

Por tales fines, los clientes al final del día generan:

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

Debe diseñarse como módulo desacoplado y adaptable pensando en 3 formas de traducción que interactúen mutuamente: (i) traducción total, (ii) traducción parcial de un fragmento seleccionado, (iii) traducción por sugerencia.

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

### Pasarela de pagos

#### Flujo économico planteado
Traductor → Pasarela de pagos → Plataforma

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
