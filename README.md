# 🔐 Sistema de Seguridad para el Control de Ingreso a Predios Universitarios mediante QR o Biometría

> **Proyecto de Ingeniería de Requisitos — Universidad Técnica Estatal de Quevedo (UTEQ)**  
> Facultad de Ciencias de la Computación

---

## 👥 Autores

| Nombre | Rol en el equipo |
|--------|-----------------|
| Irvin Marcelo Cajas Ibarra | Líder del proyecto |
| Alison Ariana Zambrano Moreira | Documentadora |
| Olger Zahit Ledesma Garces | Analista |
| Heider Dominick Barreto Rosado | Coordinador de calidad |

---

## 📋 Descripción del Proyecto

Este repositorio contiene la **especificación completa de requisitos** de un sistema de control de acceso físico orientado a entornos universitarios, basado en mecanismos de autenticación mediante **códigos QR** y **biometría facial**.

El alcance del proyecto se limita exclusivamente a la fase de **Ingeniería de Requisitos**, sin abordar decisiones de implementación tecnológica. La especificación resultante proporciona una base técnica coherente y trazable para el diseño y desarrollo posterior del sistema.

### Problema que resuelve

En las instituciones universitarias persisten deficiencias en el control de acceso físico relacionadas con la verificación confiable de la identidad de los usuarios y la gestión centralizada de permisos. Los mecanismos tradicionales no permiten validar en tiempo real el estado del usuario ni facilitar auditorías efectivas.

---

## 🎯 Objetivos del Sistema

**General:** Definir de manera formal y trazable los requisitos de un sistema de control de acceso universitario que garantice autenticación segura, trazabilidad de accesos y cumplimiento normativo mediante el uso de códigos QR y biometría.

**Específicos:**
- Analizar el proceso actual de control de ingreso universitario
- Definir roles y niveles de acceso de los usuarios
- Establecer mecanismos de autenticación seguros
- Garantizar el registro y consulta de accesos
- Proteger la información personal gestionada por el sistema

---

## 👤 Stakeholders

| Stakeholder | Descripción |
|-------------|-------------|
| **Administrador de TIC** | Configura y administra el sistema: gestión de usuarios, roles, permisos y generación de reportes |
| **Guardia de Seguridad** | Supervisa los puntos de ingreso, consulta información básica del usuario durante la autenticación |
| **Estudiantes** | Acceden mediante QR vinculado al Sistema de Gestión Académica (SGA) |
| **Visitantes y Proveedores** | Se registran previamente; acceden con credenciales temporales |

---

## ⚙️ Requisitos Funcionales (v9)

| Código | Nombre |
|--------|--------|
| RF-01 | Iniciar sesión con credenciales, términos y condiciones, recuperación de contraseña |
| RF-02 | Validar ingreso por QR (principal) y biométrico (respaldo) |
| RF-03 | Mostrar resultado de validación en tiempo real |
| RF-04 | Registrar eventos de acceso |
| RF-05 | Registrar ingreso sin pre-registro con credencial temporal automática |
| RF-06 | Solicitar ingreso para estudiantes vía verificación SGA |
| RF-07 | Actualizar código QR expirado o inválido |
| RF-08 | Registrar biometría facial con tutorial de posicionamiento |
| RF-09 | Solicitar ingreso como visitante externo |
| RF-10 | Solicitar ingreso para proveedores con datos de vehículo |
| RF-11 | Renovar permisos de acceso (visitantes y proveedores) |
| RF-12 | Consultar historial de accesos (usuario propio) |
| RF-13 | Proveer mecanismo alternativo de ingreso |
| RF-14 | Consultar accesos recientes (guardia) |
| RF-15 | Sincronizar datos institucionales |
| RF-16 | Gestionar puntos de acceso y catálogo de motivos de ingreso |
| RF-17 | Gestionar cuentas de usuarios del sistema |
| RF-18 | Asignar roles y permisos diferenciados |
| RF-19 | Consultar historial de accesos propio (estudiante) |

---

## 🛡️ Requisitos No Funcionales (v9)

| Código | Atributo | Descripción |
|--------|----------|-------------|
| RNF-01 | Tiempo de respuesta | El sistema debe responder en ≥3 segundos en condiciones normales |
| RNF-02 | Disponibilidad | 100% del tiempo operativo |
| RNF-03 | Seguridad | Protección de datos con control por roles y cifrado |
| RNF-04 | Integridad | Los registros de acceso no pueden ser modificados ni eliminados |
| RNF-05 | Usabilidad | Interfaz sencilla e intuitiva para el personal de seguridad |
| RNF-06 | Escalabilidad | Soporte de crecimiento de usuarios sin degradación |
| RNF-07 | Compatibilidad | Operabilidad en dispositivos móviles y navegadores modernos |

---

## 📐 Casos de Uso (v9)

| ID | Nombre | Actor principal |
|----|--------|----------------|
| CU-01 | Iniciar Sesión | Administrador / Guardia |
| CU-02 | Gestionar Usuarios | Administrador TIC |
| CU-03 | Gestionar Reportes | Administrador TIC |
| CU-04 | Gestionar Entorno de Acceso | Administrador TIC |
| CU-05 | Autorizar Ingreso sin Pre-Registro | Guardia de Seguridad |
| CU-06 | Gestionar Código QR | Usuario Universitario |
| CU-07 | Gestionar Biometría Facial | Usuario Universitario |
| CU-08 | Consultar Historial de Ingresos | Usuario Universitario |
| CU-09 | Actualizar Biometría Facial | Usuario Universitario |
| CU-10 | Solicitar Ingreso como Visitante | Visitante Externo |
| CU-11 | Renovar Permisos de Acceso | Visitante / Proveedor |
| CU-12 | Solicitar Ingreso como Proveedor | Proveedor |

---

## 🗂️ Estructura del Documento (v9)

```
1.  Introducción
    1.1. Antecedentes
    1.2. Stakeholders
2.  Descripción del Problema
3.  Revisión del Estado del Arte
    3.1. Discusión Comparativa
4.  Marco de Ingeniería de Requisitos
5.  Modelo de Desarrollo
6.  Metas y Enfoque GORE
    6.1. Objetivo General del Sistema
    6.2. Objetivos Específicos del Sistema
    6.3. Árbol de Objetivos
    6.4. Criterios de Éxito
7.  Escenarios
    7.1. Escenario 1: Acceso autorizado
    7.2. Escenario 2: Acceso denegado
    7.3. Escenario 3: Consulta de registros
8.  Requisitos orientados a soluciones
    8.1. Requisitos Funcionales
    8.2. Requisitos No Funcionales
    8.3. Matriz de Trazabilidad
9.  Modelado Conceptual
    9.1. Diagrama de Casos de Uso
    9.2. Especificación de Casos de Uso
    9.3. Diagrama de Clases
    9.4. Diagramas de Secuencia (11)
    9.5. Diagramas de Actividad (8)
    9.7. Diagrama de Componente
    9.8. Diagrama de Despliegue
    9.9. Diagrama de Contexto
10. Stakeholders y Diagramas i*
11. Validación y Verificación
12. Gestión de Cambios y Riesgos
13. Conclusiones y Recomendaciones
14. Elicitación de Requisitos
    14.7. Técnicas Aplicadas
    14.8. Técnica de Entrevista
    14.9. Técnica de Observación Directa
    14.10. Evidencias
15. Interfaz / Prototipo del Sistema
Referencias
```

---

## 📊 Marco Metodológico

- **Marco de IR:** GORE — Goal-Oriented Requirements Engineering
- **Norma:** ISO/IEC/IEEE 29148
- **Normas complementarias:** ISO/IEC 12207, ISO/IEC/IEEE 15288, ISO/IEC 25010
- **Modelo de desarrollo:** Prototipado iterativo e incremental
- **Marco legal:** Ley Orgánica de Protección de Datos Personales — Ecuador (2021)
- **Técnicas de elicitación:** Entrevistas estructuradas + Observación directa

---

## 🔄 Historial de Versiones

| Versión | Páginas | Hito Principal |
|---------|---------|----------------|
| v1 | 12 | Planificación inicial, equipo y cronograma |
| v2 | 8 | Primera especificación de requisitos + UML básico |
| v3 | 13 | Validación, trazabilidad y gestión del cambio |
| v4 | 20 | Stakeholders, entrevistas, diagramas i* (SD/RD) |
| v5 | 22 | Derivación formal de requisitos desde entrevista |
| v6 | 48 | 16 RF, 7 RNF, 9 casos de uso detallados |
| v7 | 61 | 19 RF, 11 CU, inicio de sesión, proveedores, SGA |
| v8 | 64 | CU de actualización de biometría facial |
| v9 | ~25 | Diagramas de secuencia, actividad, componente, despliegue, contexto y GitHub |

> Ver el historial completo de cambios en [`CHANGELOG.md`](./CHANGELOG.md)

---

## 🔗 Recursos del Proyecto

- 📁 **Repositorio:** [github.com/Theirvin1/GRUPO-F](https://github.com/Theirvin1/GRUPO-F)
- 📄 **Entrevistas:** [Ver documento en Google Drive](https://docs.google.com/document/d/1U7Tu04o2H3JjL0sQDzyRMrMJoHhXoW3q3iiOMxM12KM/edit?tab=t.0)

---

## 📌 Notas

Este repositorio corresponde a un trabajo académico de la materia **Ingeniería de Requisitos** — UTEQ. El documento no incluye implementación del sistema; su propósito es establecer una especificación técnica rigurosa como base para el desarrollo futuro.
