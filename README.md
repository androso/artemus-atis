# Artemus App — Sistema de Distribución de Vivienda 2D

> **Proyecto Integrador ATIS — Universidad de Oriente (UNIVO)**  
> **Laboratorio 2 — Planificación Inicial, Gestión de Backlog y Sprint 0**  
> **Tablero de GitHub Projects:** [Artemus App — Sprint 0](https://github.com/users/androso/projects/9)

---

## 1. Descripción del Producto

**Artemus** es una aplicación web interactiva de diseño y distribución arquitectónica residencial en dos dimensiones (2D). Permite a propietarios y arquitectos ingresar dimensiones de terreno, definir el programa arquitectónico residencial y registrar preferencias estéticas y funcionales para generar de manera automatizada propuestas conceptuales de layouts habitables, iterar sobre alternativas, aceptar una propuesta y exportarla a formatos profesionales (PDF y DXF), incorporando una etapa formal de revisión técnica por arquitectos colegiados.

---

## 2. Equipo de Trabajo y Distribución de Responsabilidades

El equipo del proyecto integrador está compuesto por los siguientes integrantes, con distribución de roles ágiles y autoría de 2 historias de usuario por integrante:

| Integrante | Rol Scrum | Responsabilidad Principal | Historias a Cargo |
|---|---|---|---|
| **Steisy Benítez** | Product Owner (PO) | Definición de visión de producto, requerimientos de cliente y priorización de negocio | US-01, US-02 |
| **Anderson Fuentes** | Scrum Master (SM) | Facilitación de ceremonias ágiles, eliminación de impedimentos y gestión de tableros | US-03, US-04 |
| **Aníbal Campos** | Developer | Arquitectura de software, motor de generación 2D e interactividad en canvas | US-05, US-06 |
| **Elmer Garcia** | Developer | Flujos de formalización, exportación documental PDF e interoperabilidad DXF | US-07, US-08 |
| **Isaac Medrano** | Developer | Consola de auditoría técnica del arquitecto y consolidación de requisitos | US-09, US-10 |

> *Nota de evaluación:* Conforme a las directrices del Laboratorio 2, las historias **US-01 a US-08** representan el conjunto base obligatorio de 8 historias de usuario para un equipo de 4 integrantes. Se incorporan **US-09 y US-10** para cubrir la totalidad de los 5 integrantes del equipo ATIS.

---

## 3. Configuración del Tablero en GitHub Projects

El tablero oficial del proyecto está configurado en **GitHub Projects (v2)** bajo el nombre **Artemus App — Sprint 0**:

- **URL del Tablero:** [https://github.com/users/androso/projects/9](https://github.com/users/androso/projects/9)
- **Columnas de Flujo de Trabajo:**
  1. `Backlog` (Elementos listos para ser refinados o seleccionados para desarrollo).
  2. `En progreso` (Elementos en desarrollo activo).
  3. `En revisión` (Pull Requests en revisión técnica de pares y validación funcional).
  4. `Hecho` (Elementos que cumplen en su totalidad la *Definition of Done*).
- **Campos Personalizados Configurados:**
  - `Prioridad`: Tipo selección única (`Alta`, `Media`, `Baja`).
  - `Story Points`: Tipo numérico (Escala Fibonacci acordada en Planning Poker: 1, 2, 3, 5, 8, 13).
  - `Status`: Tipo selección única (`Backlog`, `En progreso`, `En revisión`, `Hecho`).

---

## 4. Planificación del Sprint 0

### 4.1. Objetivo del Sprint 0 (*Sprint Goal*)
> *"Establecer la infraestructura base, arquitectura del sistema, entorno de desarrollo y la implementación del núcleo de captura de requisitos residenciales (autenticación segura, dimensiones del terreno, programa de espacios y preferencias arquitectónicas), dejando el backlog priorizado, estimado y validado para la generación del layout 2D."*

### 4.2. Elementos Seleccionados para el Sprint 0
Para el Sprint 0 se seleccionaron **5 historias de usuario fundamentales** que totalizan **24 Story Points**:

| ID | Historia de Usuario | Responsable | Prioridad | Story Points | Justificación para Sprint 0 |
|---|---|---|:---:|:---:|---|
| **US-01** | Registro e inicio de sesión | Steisy Benítez | Alta | 5 | Base de autenticación, seguridad y control de acceso basado en roles (RBAC). |
| **US-02** | Registrar terreno del proyecto | Steisy Benítez | Alta | 5 | Modelo dimensional y restricciones geométricas indispensables para todo el sistema. |
| **US-03** | Definir espacios y habitaciones | Anderson Fuentes | Alta | 8 | Catálogo de recintos y reglas de validación de área construible versus área de terreno. |
| **US-04** | Capturar preferencias de vivienda | Anderson Fuentes | Alta | 3 | Parámetros de estilo, plantas y estacionamiento que alimentan el algoritmo de layout. |
| **US-10** | Resumen de requisitos del proyecto | Isaac Medrano | Media | 3 | Vista consolidada para validar la integridad de los datos antes de pasar a la generación 2D. |

*Total Sprint 0:* **24 Story Points**  
*Total Product Backlog:* **58 Story Points** (10 historias) / **50 Story Points** (8 historias base).

---

## 5. Definition of Done (DoD) Común

Toda historia de usuario del proyecto Artemus debe cumplir obligatoriamente los siguientes criterios para transicionar a la columna **Hecho**:

1. **Criterios de Aceptación Verificados:** Todos los criterios de aceptación individuales definidos en la historia de usuario han sido probados y aprobados por el Product Owner y el equipo de pruebas.
2. **Estándares de Código y Linter:** El código fuente respeta la guía de estilos establecida, no genera advertencias críticas de linter ni errores de compilación/transpilación.
3. **Pruebas Automatizadas:** Se han implementado y ejecutado pruebas unitarias e integrales para la lógica de negocio, con una cobertura mínima del 80% sobre los módulos impactados.
4. **Revisión de Código (*Code Review*):** Todo cambio ha sido canalizado a través de un Pull Request con la aprobación de al menos un revisor técnico independiente del autor.
5. **Documentación Técnica:** El código cuenta con documentación interna de funciones clave, endpoints API documentados y el ticket/issue correspondiente en GitHub actualizado con notas técnicas.
6. **Despliegue en Entorno de Pruebas:** La funcionalidad está desplegada y operativa en el entorno de staging/pruebas sin provocar regresiones en funcionalidades existentes.

---

## 6. Backlog de Historias de Usuario

A continuación se detallan las 10 historias de usuario creadas, vinculadas a los issues `#1` a `#10` de este repositorio y reflejadas en el tablero de GitHub Projects:

### Resumen Consolidado

| ID | Título | Actor | Prioridad | SP | Responsable | Estado Inicial |
|:---:|---|---|:---:|:---:|---|:---:|
| **US-01** | Registro e inicio de sesión | Propietario / Arquitecto | Alta | 5 | Steisy Benítez | Backlog (Sprint 0) |
| **US-02** | Registrar terreno del proyecto | Propietario | Alta | 5 | Steisy Benítez | Backlog (Sprint 0) |
| **US-03** | Definir espacios y habitaciones | Propietario | Alta | 8 | Anderson Fuentes | Backlog (Sprint 0) |
| **US-04** | Capturar preferencias de vivienda | Propietario | Alta | 3 | Anderson Fuentes | Backlog (Sprint 0) |
| **US-05** | Generar propuesta conceptual 2D | Propietario | Alta | 13 | Aníbal Campos | Backlog |
| **US-06** | Editar y regenerar el layout | Propietario | Media | 8 | Aníbal Campos | Backlog |
| **US-07** | Aceptar propuesta conceptual | Propietario | Alta | 3 | Elmer Garcia | Backlog |
| **US-08** | Exportar a PDF y DXF | Propietario / Arquitecto | Alta | 8 | Elmer Garcia | Backlog |
| **US-09** | Revisión por arquitecto | Arquitecto | Media | 5 | Isaac Medrano | Backlog |
| **US-10** | Resumen de requisitos del proyecto | Propietario / Arquitecto | Media | 3 | Isaac Medrano | Backlog (Sprint 0) |

---

### Detalle de las Historias de Usuario

#### US-01 — Registro e inicio de sesión
- **Issue:** [#1](https://github.com/androso/artemus-atis/issues/1)
- **Actor:** Propietario o Arquitecto
- **Necesidad:** Registrarse e iniciar sesión con correo electrónico y contraseña.
- **Beneficio:** Acceder a mis proyectos y funcionalidades según mi rol en el sistema.
- **Prioridad:** Alta | **Estimación:** 5 SP | **Responsable:** Steisy Benítez (PO)
- **Criterios de Aceptación:**
  1. *Validación de credenciales:* Si las credenciales son incorrectas, el sistema muestra un mensaje de error claro ("Credenciales inválidas") y deniega el acceso sin exponer detalles del error en el servidor.
  2. *Control de acceso por rol:* Tras autenticarse correctamente, el sistema redirige al usuario al panel de control correspondiente a su rol (vista de proyectos residenciales para propietarios o consola de revisión técnica para arquitectos).
  3. *Validación de formato y seguridad:* El sistema valida que el correo cumpla formato estándar RFC 5322 y que la contraseña posea un mínimo de 8 caracteres (al menos una mayúscula, un número y un símbolo especial) antes de enviar la solicitud.
  4. *Persistencia y expiración de sesión:* La sesión genera un token seguro (JWT) almacenado de forma protegida; la sesión expira tras 60 minutos de inactividad o de inmediato al cerrar sesión voluntariamente.

#### US-02 — Registrar terreno del proyecto
- **Issue:** [#2](https://github.com/androso/artemus-atis/issues/2)
- **Actor:** Propietario
- **Necesidad:** Ingresar frente, fondo, área total y orientación cardinal del terreno.
- **Beneficio:** Que la propuesta arquitectónica conceptual se adapte a las dimensiones físicas reales.
- **Prioridad:** Alta | **Estimación:** 5 SP | **Responsable:** Steisy Benítez (PO)
- **Criterios de Aceptación:**
  1. *Validación dimensional:* El sistema rechaza valores menores o iguales a cero en frente, fondo o área total, mostrando mensajes de error en los campos respectivos y bloqueando el registro.
  2. *Consistencia geométrica:* El área total ingresada no puede diferir en más de un margen configurable respecto a la multiplicación de frente por fondo para terrenos regulares, alertando al usuario ante inconsistencias geométricas.
  3. *Orientación cardinal obligatoria:* El usuario debe seleccionar obligatoriamente la orientación cardinal del frente (Norte, Sur, Este u Oeste), la cual queda vinculada a la orientación espacial del layout.
  4. *Persistencia y asociación:* Al guardar, los datos del terreno quedan enlazados unívocamente al proyecto activo y se reflejan de inmediato en el resumen de requisitos.

#### US-03 — Definir espacios y habitaciones
- **Issue:** [#3](https://github.com/androso/artemus-atis/issues/3)
- **Actor:** Propietario
- **Necesidad:** Indicar los espacios requeridos indicando tipo, cantidad y área deseada.
- **Beneficio:** Comunicar mis necesidades funcionales y de distribución del hogar.
- **Prioridad:** Alta | **Estimación:** 8 SP | **Responsable:** Anderson Fuentes (SM)
- **Criterios de Aceptación:**
  1. *Catálogo de espacios zonificados:* El usuario puede seleccionar habitaciones de una lista clasificada en zonas (social: sala/comedor; privada: dormitorios; servicio: cocina/baños) o crear un espacio personalizado con nombre válido.
  2. *Operaciones CRUD en borrador:* El usuario puede agregar, editar dimensiones/cantidades y eliminar espacios antes de generar la distribución 2D.
  3. *Regla de área útil y advertencia:* Si la suma de las áreas deseadas supera el área máxima construible del terreno, el sistema emite una advertencia visual de sobreocupación indicando el exceso en m².
  4. *Restricciones mínimas habitables:* Cada espacio debe poseer un área mínima reglamentaria mayor a cero (ej. mínimo 9 m² para dormitorios principales y 3 m² para baños completos).

#### US-04 — Capturar preferencias de vivienda
- **Issue:** [#4](https://github.com/androso/artemus-atis/issues/4)
- **Actor:** Propietario
- **Necesidad:** Registrar estilo arquitectónico, número de plantas, plazas de estacionamiento y previsión de ampliación.
- **Beneficio:** Orientar la generación del layout según mis expectativas de vida y crecimiento.
- **Prioridad:** Alta | **Estimación:** 3 SP | **Responsable:** Anderson Fuentes (SM)
- **Criterios de Aceptación:**
  1. *Campos requeridos y rangos válidos:* El formulario exige seleccionar el número de plantas (mínimo 1, máximo 3) y la cantidad de plazas de estacionamiento (mínimo 0) antes de habilitar la generación del diseño.
  2. *Selección de estilo y ampliación futura:* El usuario selecciona el estilo arquitectónico deseado y marca si requiere dejar previstas áreas o núcleos estructurales para futuras ampliaciones.
  3. *Distribución por niveles:* Si el usuario elige dos o más plantas, el sistema permite definir qué espacios se asignan preferentemente a planta baja o a plantas superiores.
  4. *Consolidación en ficha técnica:* Todas las preferencias quedan almacenadas y asociadas al proyecto, mostrándose en el resumen de requisitos.

#### US-05 — Generar propuesta conceptual 2D
- **Issue:** [#5](https://github.com/androso/artemus-atis/issues/5)
- **Actor:** Propietario
- **Necesidad:** Generar una distribución conceptual 2D a partir del terreno, los espacios y las preferencias definidas.
- **Beneficio:** Visualizar una alternativa arquitectónica funcional y clara de mi vivienda.
- **Prioridad:** Alta | **Estimación:** 13 SP | **Responsable:** Aníbal Campos (Dev)
- **Criterios de Aceptación:**
  1. *Validación previa de requisitos:* El sistema verifica que existan datos válidos de terreno, al menos un área social, un dormitorio y un baño antes de iniciar el cálculo; si falta información, bloquea la acción y señala los pendientes.
  2. *Disposición poligonal sin solapes:* El motor coloca los recintos dentro de los límites del terreno sin superposición física entre habitaciones, respetando retiros de linderos e insertando circulaciones de conexión.
  3. *Renderizado 2D y versionado:* El plano se dibuja en un canvas interactivo 2D con etiquetas de nombres y áreas por habitación, generando automáticamente un código de versión inmutable (ej. Layout v1.0).
  4. *Balance dimensional:* La interfaz muestra un panel comparativo entre el área solicitada por el usuario y el área real obtenida en la propuesta generada.

#### US-06 — Editar y regenerar el layout
- **Issue:** [#6](https://github.com/androso/artemus-atis/issues/6)
- **Actor:** Propietario
- **Necesidad:** Ajustar manualmente la posición o dimensiones de las habitaciones o regenerar una propuesta alternativa.
- **Beneficio:** Acercar el diseño a mis necesidades particulares antes de aceptarlo formalmente.
- **Prioridad:** Media | **Estimación:** 8 SP | **Responsable:** Aníbal Campos (Dev)
- **Criterios de Aceptación:**
  1. *Edición interactiva con detección de colisiones:* El usuario puede arrastrar y reacomodar habitaciones en el canvas; si un recinto invade otro o excede el límite del terreno, el sistema alerta visualmente en color rojo y bloquea el guardado.
  2. *Historial inmutable de versiones:* Cada acción de regeneración o guardado de edición crea una nueva versión secuencial (v1.1, v1.2, v2.0) sin sobreescribir ni eliminar las versiones anteriores.
  3. *Comparador y retorno de versiones:* El usuario puede navegar entre las versiones generadas y restaurar cualquier versión anterior como la versión activa de trabajo.

#### US-07 — Aceptar propuesta conceptual
- **Issue:** [#7](https://github.com/androso/artemus-atis/issues/7)
- **Actor:** Propietario
- **Necesidad:** Marcar formalmente una versión de propuesta como aceptada.
- **Beneficio:** Habilitar su exportación técnica y la posterior revisión por parte del arquitecto.
- **Prioridad:** Alta | **Estimación:** 3 SP | **Responsable:** Elmer Garcia (Dev)
- **Criterios de Aceptación:**
  1. *Restricción de estado inicial:* Solo se puede aceptar una versión que se encuentre en estado válido (generada o editada) y libre de conflictos o colisiones espaciales.
  2. *Bloqueo contra modificaciones posteriores:* Al aceptar, la propuesta seleccionada se congela en modo de solo lectura y cambia su estado a "Aceptada — Pendiente de revisión".
  3. *Modal de confirmación explícita:* El sistema solicita confirmación mediante un cuadro de diálogo antes de ejecutar el cambio de estado, notificando al usuario que la versión quedará bloqueada.
  4. *Habilitación de acciones posteriores:* Al completar la aceptación, se desbloquean automáticamente los botones de exportación (PDF/DXF) y el envío a la bandeja de revisión del arquitecto.

#### US-08 — Exportar a PDF y DXF
- **Issue:** [#8](https://github.com/androso/artemus-atis/issues/8)
- **Actor:** Propietario o Arquitecto
- **Necesidad:** Exportar la propuesta aceptada en formatos PDF de presentación y DXF editable.
- **Beneficio:** Disponer de documentación formal impresa y facilitar el modelado en herramientas CAD profesionales.
- **Prioridad:** Alta | **Estimación:** 8 SP | **Responsable:** Elmer Garcia (Dev)
- **Criterios de Aceptación:**
  1. *Documento PDF estructurado:* El archivo PDF exportado incluye carátula con datos del proyecto, cuadro resumen de requerimientos y el plano 2D acotado con escala gráfica legible.
  2. *Formato DXF estandarizado por capas:* El archivo DXF organiza los elementos en capas normalizadas (MUROS, PUERTAS, VENTANAS, TEXTOS, COTAS) en escala métrica 1:1.
  3. *Generación descargable y validada:* Los archivos se descargan desde el navegador con nomenclatura estandarizada (`[Proyecto]_[Version]_[Fecha].pdf/dxf`) y abren sin errores de sintaxis en visores estándar (Acrobat Reader, AutoCAD, LibreCAD).

#### US-09 — Revisión por arquitecto
- **Issue:** [#9](https://github.com/androso/artemus-atis/issues/9)
- **Actor:** Arquitecto
- **Necesidad:** Auditar técnicamente una propuesta aceptada y emitir un dictamen formal con observaciones.
- **Beneficio:** Validar la factibilidad constructiva y orientar al cliente en ajustes previos al diseño final.
- **Prioridad:** Media | **Estimación:** 5 SP | **Responsable:** Isaac Medrano (Dev)
- **Criterios de Aceptación:**
  1. *Acceso a ficha técnica completa:* El arquitecto puede visualizar el plano 2D aceptado, especificaciones del terreno, listado de espacios y memoria de preferencias en una sola vista de auditoría.
  2. *Opciones de dictamen regladas:* El arquitecto puede seleccionar exclusivamente entre dos dictámenes: "Aprobado" o "Requiere Ajustes".
  3. *Observaciones técnicas obligatorias:* Si el dictamen es "Requiere Ajustes", el sistema exige ingresar comentarios técnicos detallados (mínimo 20 caracteres) antes de permitir el registro.
  4. *Registro de auditoría y notificación:* El dictamen queda registrado con fecha, hora e identificación del arquitecto, y se notifica al propietario para su consulta en el sistema.

#### US-10 — Resumen de requisitos del proyecto
- **Issue:** [#10](https://github.com/androso/artemus-atis/issues/10)
- **Actor:** Propietario o Arquitecto
- **Necesidad:** Consultar un resumen técnico estructurado de terreno, programa arquitectónico y preferencias.
- **Beneficio:** Auditar de forma integral la coherencia de los datos del proyecto antes y después del diseño.
- **Prioridad:** Media | **Estimación:** 3 SP | **Responsable:** Isaac Medrano (Dev)
- **Criterios de Aceptación:**
  1. *Consolidación en vista única:* La pantalla agrupa de forma clara los datos del terreno, la lista tabular de espacios (con totales de metros cuadrados) y las preferencias de diseño.
  2. *Alertas de datos pendientes o discordantes:* El sistema evalúa y resalta en amarillo advertencias si faltan campos recomendados o si detecta desproporción entre áreas de espacios y tamaño del terreno.
  3. *Navegación directa para correcciones:* Cada bloque del resumen dispone de un botón directo de edición que conduce al formulario específico sin perder el contexto del proyecto.

---

## 7. Proceso de Estimación (Planning Poker)

El equipo aplicó la técnica de **Planning Poker** utilizando la secuencia de Fibonacci modificada (1, 2, 3, 5, 8, 13). Durante la sesión:
1. Se identificaron y eliminaron ambigüedades en la descripción del valor y los criterios de aceptación.
2. Se resolvió la división de funcionalidades grandes, manteniendo la generación del plano (US-05) como la tarea algorítmica de mayor peso (13 SP).
3. Se llegó a un consenso unánime sobre los valores finales registrados en las tarjetas y campos de GitHub Projects.
