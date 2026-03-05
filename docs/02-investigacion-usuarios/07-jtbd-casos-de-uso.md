---

# 7. Jobs-to-be-Done / Casos de Uso

## Introducción

El presente apartado describe los Jobs-to-be-Done (JTBD) y los casos de uso principales del sistema, permitiendo identificar las tareas que los usuarios necesitan realizar dentro de la aplicación.

El sistema prioriza la seguridad y confidencialidad de la información mediante autenticación segura y almacenamiento local.

---

## Jobs-to-be-Done (JTBD)

| ID | Usuario | Necesidad | Resultado Esperado |
|----|---------|-----------|--------------------|
| JTBD-01 | Usuario autorizado | Acceder al sistema de forma segura | Acceso validado mediante cuenta Google |
| JTBD-02 | Usuario autorizado | Consultar archivos confidenciales | Visualización segura de archivos |
| JTBD-03 | Administrador | Gestionar permisos de acceso | Control adecuado de usuarios |
| JTBD-04 | Usuario autorizado | Manipular archivos localmente | Protección de información sensible |

---

## Casos de Uso

### CU-01 — Inicio de Sesión
**Actor:** Usuario  

1. El usuario abre la aplicación.  
2. Selecciona iniciar sesión.  
3. Se autentica mediante Google.  
4. El sistema valida identidad.  
5. Se concede acceso.

**Resultado:** Usuario autenticado.

---

### CU-02 — Acceso a Archivos
**Actor:** Usuario autorizado  

1. Usuario inicia sesión.  
2. Accede al módulo de archivos.  
3. Selecciona archivo.  
4. Sistema valida permisos.  
5. Archivo es mostrado.

**Resultado:** Acceso controlado.

---

### CU-03 — Gestión de Accesos
**Actor:** Administrador  

1. Administrador inicia sesión.  
2. Accede al panel de usuarios.  
3. Modifica permisos.  
4. Guarda cambios.

**Resultado:** Permisos actualizados.

---

### CU-04 — Cierre de Sesión
**Actor:** Usuario  

1. Usuario selecciona cerrar sesión.  
2. Sistema finaliza sesión activa.  
3. Regresa a pantalla inicial.

**Resultado:** Sistema protegido.
