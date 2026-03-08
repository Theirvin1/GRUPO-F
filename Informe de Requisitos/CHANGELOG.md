# CHANGELOG

## Sistema de Seguridad para el Control de Ingreso a Predios Universitarios mediante QR o Biometría

**Proyecto:** Ingeniería de Requisitos — UTEQ  
**Autores:** Heider Barreto, Irvin Cajas, Olger Ledesma, Alison Zambrano  
**Materia:** Ingeniería de Requisitos

---

## [v1] — Planificación Inicial del Proyecto

**Páginas:** 12

### Agregado
- Documento de planificación inicial del proyecto titulado **"TA-PFC Planificación"**
- Definición del título del proyecto: *Sistema avanzado de control de ingreso universitario con QR, biometría y validación segura en tiempo real*
- Establecimiento del **objetivo general** y **objetivos específicos** del proyecto
- Descripción del sistema y del problema: limitaciones de los métodos tradicionales de control de ingreso
- Identificación de los **actores principales**: Administrador del sistema, Usuario universitario y Personal de seguridad
- Definición de las **fuentes de información** (artículos científicos, documentación institucional)
- Selección de la **metodología iterativa** como marco de trabajo
- **Cronograma del proyecto** de 17 semanas
- Definición de **roles y responsabilidades** del equipo: Líder (Irvin Cajas), Documentador (Alison Zambrano), Analista (Olger Ledesma), Coordinador de calidad (Heider Barreto)
- Referencias normativas aplicadas: ISO/IEC/IEEE 29148, ISO/IEC 12207, ISO/IEC/IEEE 15288, ISO/IEC 25010
- Reglas de trabajo: comunicación por WhatsApp, control de versiones con fechas de modificación
- Anexos: organización del equipo, definición del alcance inicial, metodología elegida y entorno colaborativo

---

## [v2] — Especificación Inicial de Requisitos y Modelado Base

**Páginas:** 8

### Agregado
- Cambio de formato: de documento de planificación a **artículo técnico académico** con resumen
- Sección de **Descripción del Problema** con análisis de limitaciones de sistemas QR puros y biométricos
- **Revisión del Estado del Arte** con análisis de trabajos previos sobre control de acceso en entornos educativos
- Adopción del marco **GORE (Goal-Oriented Requirements Engineering)** como marco de trabajo
- Sección **Metas y Enfoque GORE** con árbol jerárquico de objetivos (Figura 1)
- Definición de **criterios de éxito** del sistema
- **3 escenarios de uso** básicos: acceso autorizado, acceso denegado y consulta de registros
- **5 Requisitos Funcionales** iniciales (RF1–RF5): registro de usuarios, generación de QR, autenticación biométrica, registro de accesos, generación de reportes
- **4 Requisitos No Funcionales** iniciales (RNF1–RNF4): protección de datos, tiempo de respuesta ≤2 seg, control por roles, interfaz usable
- **Glosario** de términos: Autenticación, Biometría, Código QR, Trazabilidad
- **Diagrama de Casos de Uso** (Figura 2)
- **Diagrama de Clases** (Figura 3)
- Referencias actualizadas incluyendo Ley Orgánica de Protección de Datos Personales (Ecuador, 2021)

---

## [v3] — Especificación Completa con Validación y Trazabilidad

**Páginas:** 13

### Agregado
- Título actualizado: *"Sistema avanzado de control de ingreso universitario con códigos QR y biometría: Especificación de Requisitos"*
- Alineación explícita con la norma **ISO/IEC/IEEE 29148**
- **Diccionario de Datos** con definición formal de entidades: Usuario, Rol, Código QR, Dato Biométrico, Registro de Acceso
- Sección de **Validación y Verificación** con técnicas de inspección, walkthroughs y revisiones cruzadas
- Subsecciones de **Hallazgos Identificados** y **Correcciones Aplicadas** durante la validación
- Sección de **Trazabilidad y Gestión del Cambio** con matriz de trazabilidad (GORE ↔ RF ↔ RNF ↔ Escenarios ↔ UML)
- **Priorización de Requisitos** según criterios de seguridad institucional, criticidad operativa y dependencia funcional
- Mecanismo de **control de versiones** y gestión del cambio documental
- Sección de **Resultados y Discusión** con análisis de cobertura de requisitos
- Análisis de **conflictos identificados y resueltos**: política diferenciada QR para estudiantes vs. biometría para externos
- **Riesgos Remanentes** identificados: datos biométricos, factor humano en identificación visual
- Sección de **Conclusiones y Recomendaciones**
- **Anexos**: Matriz de Trazabilidad y Evidencias de Validación

### Modificado
- Reformulación de requisitos no funcionales incorporando métricas verificables
- Inclusión de criterios de aceptación explícitos en todos los escenarios
- Ajustes de redacción para asegurar atomicidad y verificabilidad

---

## [v4] — Incorporación de Stakeholders, Entrevistas y Diagramas i*

**Páginas:** 20

### Agregado
- Sección **1.1 Stakeholders** con clasificación formal en tres grupos: Administrador TIC, Personal de seguridad, Estudiantes y personas externas
- Descripción detallada de la integración **híbrida QR + biometría** y su justificación comparativa
- **Diagrama de Dependencia Estratégica (SD)** — Figura 4: modelado de relaciones entre actores del sistema
- **Diagrama de Racional Estratégico (RD)** — Figura 5: descomposición interna de metas y tareas por actor
- **Cuestionario de entrevista al Guardia de Seguridad** (13 preguntas)
- **Enlace a la entrevista en video** (Google Drive)
- **Técnicas de Elicitación Aplicadas**: entrevistas y observación directa
- **Derivación de requisitos** a partir de la entrevista: identificación de criterios de acceso, información requerida, riesgos
- Requisitos funcionales RF1–RF5 reformulados con mayor detalle (actor explícito, descripción precisa)
- RNF reformulados: RNF1 (Seguridad con control por roles), RNF2 (Rendimiento ≤2 seg), RNF3 (Legal y Trazabilidad)

### Modificado
- Escenarios de uso ampliados con **precondiciones, flujos principales, flujos alternativos y postcondiciones** completos
- Discusión Comparativa del Estado del Arte expandida

---

## [v5] — Consolidación con Derivación de Requisitos desde Entrevista

**Páginas:** 22

### Agregado
- Sección **13.1 Derivación de Requisitos a partir de la Entrevista** con análisis sistemático pregunta por pregunta (P3, P6, P12, P5, P4, P11)
- Nuevos requisitos funcionales derivados de la entrevista:
  - RF: Mostrar información básica del usuario autenticado (nombre, foto, carrera, estado)
  - RF: Registrar información de visitantes y proveedores con evidencia de ingreso/salida
  - RF: Denegar acceso y registrar evento ante usuario no identificable
- Nuevos requisitos no funcionales derivados de la entrevista:
  - RNF: Trazabilidad de todos los intentos de acceso
  - RNF: Tiempo de respuesta acotado en horas de alta concurrencia
  - RNF: Interfaz sencilla para personal de seguridad
- **Conclusión de la Elicitación** como sección formal
- Referencias ampliadas incluyendo Ferrari & Gnesi (2021), Gotel et al. (2022) y Ahmad & Bruel (2023)

### Modificado
- Reorganización del documento: los anexos de entrevista y cuestionario se integran en la sección 13
- Técnicas de observación directa expandidas con hallazgos específicos del campus

---

## [v6] — Expansión Masiva de Requisitos y Casos de Uso Detallados

**Páginas:** 48

### Agregado
- Nuevo título: *"Sistema de Seguridad para el control de ingreso a Predios Universitario mediante QR o Biometría"*
- **16 Requisitos Funcionales** con código, nombre, descripción, fuente y actor principal (RF-01 a RF-16)
- **7 Requisitos No Funcionales** en formato tabla con código (RNF-01 a RNF-07): Tiempo de respuesta, Disponibilidad (99%), Seguridad, Integridad, Usabilidad, Escalabilidad, Compatibilidad
- **9 Casos de Uso detallados** (CU-01 a CU-09) con ID, nombre, actor, descripción, precondiciones, postcondiciones, flujos principal y alternativo, y requisitos relacionados:
  - CU-01: Procesar solicitud de ingreso para estudiantes registrados / por registrar
  - CU-02: Procesar solicitud de ingreso para distribuidor
  - CU-03: Procesar solicitud de ingreso para visitantes externos
  - CU-04: Registrar datos biométricos del usuario
  - CU-05: Generar nueva credencial QR
  - CU-06: Autorizar ingreso excepcional para visitantes sin pre-registro
  - CU-07: Gestionar cuentas de usuarios del sistema
  - CU-08: Gestionar permisos de accesos temporales
  - CU-09: Generar reportes de acceso
- **10 diagramas de casos de uso individuales** (Figs. 1–11)
- Requisito RF-08: Gestionar usuarios (crear, modificar, eliminar)
- Requisito RF-09: Asignar roles y permisos diferenciados
- Requisito RF-10: Sincronizar datos institucionales
- Requisito RF-11: Gestionar accesos temporales para visitantes
- Requisito RF-12: Consultar historial de accesos (usuario)
- Requisito RF-13: Proveer mecanismo alternativo de ingreso
- Requisito RF-14: Consultar accesos recientes (guardia)
- Requisito RF-15: Restringir funciones administrativas

### Modificado
- RNF-01 Tiempo de respuesta: ajustado a ≥3 segundos (antes ≤2 seg)
- RNF-02 Disponibilidad: aumentado al 99% del tiempo operativo

---

## [v7] — Módulo de Autenticación, Inicio de Sesión y Casos de Uso de Proveedores

**Páginas:** 61

### Agregado
- **19 Requisitos Funcionales** (RF-01 a RF-19) con nueva estructura:
  - RF-01: Iniciar sesión con credenciales, términos y condiciones, recuperación de contraseña
  - RF-02: Validar ingreso por QR (principal) + biométrico (respaldo)
  - RF-05: Registrar ingreso sin pre-registro con generación automática de credencial temporal
  - RF-06: Solicitar ingreso para estudiantes vía verificación SGA
  - RF-07: Actualizar código QR expirado o inválido
  - RF-08: Registrar biometría facial con tutorial de posicionamiento y múltiples ángulos
  - RF-09: Solicitar ingreso como visitante externo
  - RF-10: Solicitar ingreso para proveedores con datos de vehículo
  - RF-11: Renovar permisos de acceso (visitantes y proveedores)
  - RF-16: Gestionar puntos de acceso y catálogo de motivos de ingreso
  - RF-19: Consultar historial de accesos propio (estudiante)
- **11 Casos de Uso restructurados** (CU-01 a CU-11):
  - CU-01: Iniciar Sesión (nuevo — con recuperación de contraseña y registro de usuario)
  - CU-02: Gestión de Usuarios (ampliado)
  - CU-03: Gestionar Reportes (con exportación PDF/Excel)
  - CU-04: Gestión del Entorno de Acceso (nuevo — puntos de acceso + motivos de ingreso)
  - CU-06 a CU-11: flujos completos para estudiantes, visitantes, proveedores y renovación
- RNF-02 Disponibilidad: aumentado al **100%** del tiempo operativo
- **12 diagramas de casos de uso** (Figs. 1–12)

### Modificado
- Requisito RF-03: renombrado a "Mostrar resultado de validación" con información en tiempo real
- Requisito RF-04: renombrado a "Registrar eventos de acceso" (antes RF-05)
- Los roles del sistema se restringen a: **Administrador TICS** y **Guardia de Seguridad** únicamente

---

## [v8] — Caso de Uso de Actualización de Biometría Facial

**Páginas:** 64

### Agregado
- **CU-09: Actualizar Biometría Facial** — nuevo caso de uso independiente que permite reemplazar el patrón biométrico facial previamente registrado, con confirmación previa, captura de nuevo patrón y reemplazo controlado del anterior
- Flujo alternativo en **CU-08 Registrar Biometría Facial**: opción de actualizar biometría ya existente integrada en el caso de uso de registro
- **Diagrama de caso de uso CU-09** (Fig. 10) — Actualizar Biometría Facial
- Renumeración de diagramas: CU-10 (Visitante), CU-11 (Renovar permisos), CU-12 (Proveedores)
- Total de casos de uso: **12 (CU-01 a CU-12)**

### Modificado
- Descripción del CU-08 actualizada: ahora indica explícitamente que el usuario *puede actualizar su biometría previamente registrada cuando lo considere necesario*
- Los diagramas de casos de uso se renumeran a partir de CU-09

---

## [v9] — Versión Actual: Diagramas Ampliados, Antecedentes y Repositorio GitHub

**Páginas:** ~25 (versión compacta final)

### Agregado
- **Sección 1.1 Antecedentes** — nueva sección con contexto histórico e institucional del problema
- **Sección 5: Modelo de Desarrollo** — descripción explícita del modelo de desarrollo adoptado
- Enlace al **Repositorio GitHub** del proyecto en la portada
- Nombres completos de los autores en la portada (apellidos completos incluidos)
- Mención de la universidad: *Universidad Técnica Estatal de Quevedo — Facultad de Ciencias de la Computación*
- **Sección 9.4: Diagramas de Secuencia** — 11 diagramas nuevos:
  - Iniciar Sesión, Gestionar Usuarios, Gestionar Reportes, Gestionar Entorno de Acceso, Autorizar Ingreso sin Pre-Registro, Gestionar Código QR, Gestionar Biometría Facial, Consultar Historial de Ingresos, Solicitar ingreso como Visitante, Solicitar ingreso para Proveedor, Renovar Permisos de Accesos
- **Sección 9.5: Diagramas de Actividad** — 8 diagramas nuevos:
  - Iniciar Sesión, Gestionar Usuarios, Gestionar Reportes, Gestionar Entorno de Acceso, Autorizar Ingreso sin Pre-Registro, Autorizar Ingreso para Visitantes, Autorizar Ingreso para Proveedor, Renovar Permisos de Acceso
- **Sección 9.7: Diagrama de Componente** del sistema
- **Sección 9.8: Diagrama de Despliegue** del sistema
- **Sección 9.9: Diagrama de Contexto** del sistema
- Índice completo y estructurado con numeración de secciones y paginación

### Modificado
- Restructuración del índice: la sección de Modelado Conceptual pasa a ser la sección 9 (antes sección 8)
- La sección de Metas y Enfoque GORE pasa a la sección 6 (antes sección 5)
- Los Escenarios pasan a la sección 7 (antes sección 6)
- Los Requisitos orientados a soluciones pasan a la sección 8 (antes sección 7)

---

## Resumen de Evolución del Documento

| Versión | Páginas | Hito Principal |
|---------|---------|----------------|
| v1      | 12      | Planificación inicial, equipo y cronograma |
| v2      | 8       | Primera especificación de requisitos + UML básico |
| v3      | 13      | Validación, trazabilidad y gestión del cambio |
| v4      | 20      | Stakeholders, entrevistas, diagramas i* (SD/RD) |
| v5      | 22      | Derivación formal de requisitos desde entrevista |
| v6      | 48      | 16 RF, 7 RNF, 9 casos de uso detallados |
| v7      | 61      | 19 RF, 11 CU, inicio de sesión, proveedores, SGA |
| v8      | 64      | CU de actualización de biometría facial |
| v9      | ~25     | Diagramas de secuencia, actividad, componente, despliegue, contexto y repositorio GitHub |
