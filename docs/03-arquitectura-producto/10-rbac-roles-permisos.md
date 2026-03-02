# 10. Matriz de Roles y Permisos (RBAC)

## 1. Introducción

El presente documento define la matriz de Roles y Permisos (RBAC - Role Based Access Control) del sistema.

El objetivo es controlar el acceso a funcionalidades y archivos confidenciales mediante la asignación de permisos según el rol del usuario autenticado.

El sistema prioriza la seguridad de la información mediante almacenamiento local y autenticación obligatoria con cuenta Google.

---

## 2. Objetivo

Establecer qué acciones puede realizar cada tipo de usuario dentro del sistema, garantizando el acceso controlado y la protección de la información sensible.

---

## 3. Roles del Sistema

| Rol | Descripción |
|-----|-------------|
| Usuario Autorizado | Usuario autenticado mediante cuenta Google con acceso permitido |
| Usuario No Autorizado | Usuario que aún no ha iniciado sesión |

---

## 4. Permisos Definidos

| ID | Permiso | Descripción |
|----|---------|-------------|
| P-01 | Iniciar sesión | Acceder al sistema mediante cuenta Google |
| P-02 | Consultar archivos | Visualizar archivos disponibles |
| P-03 | Acceso al sistema | Uso general de la aplicación |
| P-04 | Cerrar sesión | Finalizar sesión activa |

---

## 5. Matriz RBAC

| Rol / Permiso | P-01 Login | P-02 Consultar Archivos | P-03 Acceso Sistema | P-04 Logout |
|---------------|------------|-------------------------|---------------------|-------------|
| Usuario Autorizado | ✔ | ✔ | ✔ | ✔ |
| Usuario No Autorizado | ✔ | ✖ | ✖ | ✔ |

---

## 6. Reglas de Control de Acceso

- Todo usuario debe autenticarse mediante cuenta Google.
- No existe gestión manual de usuarios dentro del sistema.
- El acceso a archivos requiere autenticación previa.
- Los archivos permanecen almacenados localmente.
- Usuarios no autenticados no pueden acceder al contenido del sistema.

---

## 7. Consideraciones de Seguridad

- No se utiliza almacenamiento en servicios cloud.
- El control de acceso se valida en cada sesión.
- Se evita exposición de archivos confidenciales.
- El acceso depende únicamente del estado de autenticación.

---

## 8. Conclusión

La implementación de RBAC permite establecer un control claro de accesos dentro del sistema, garantizando que únicamente usuarios autenticados puedan interactuar con la información confidencial almacenada localmente.
