# Artemus App — Full Capstone Context

_Last assembled: 2026-09-28_

This file consolidates everything currently known about the **Proyecto Integrador / capstone** for **Aplicación de Técnicas de Ingeniería de Software (ATIS)** from:

- the course pages stored in Notion,
- the `ats-submitted-homeworks.zip` Canvas export,
- the submitted team-formation PDF,
- the submitted Laboratorio 2 PDF,
- the current GitHub repository and issues,
- the GitHub Projects board,
- the September UML activity PDF provided in chat,
- and the project index added to Notion.

It intentionally keeps **historical submission state**, **current GitHub state**, and **course requirements** separate when they disagree.

---

## 1. Canonical links

### Notion
- **Course page — Aplicación de Técnicas de Ingeniería de Software**  
  https://app.notion.com/p/a748067844f942cb959b723986eef896
- **Course Notes database**  
  https://app.notion.com/p/58e068086ca94feab6fe2f615a5e49a7
- **Capstone index — Proyecto Integrador — Artemus App**  
  https://app.notion.com/p/3e982a6d656181f5a032c82bea7bb0e2

### GitHub
- **Repository — `androso/artemus-atis`**  
  https://github.com/androso/artemus-atis
- **GitHub Project — Artemus App — Sprint 0 (Project #9)**  
  https://github.com/users/androso/projects/9
- **Issues / User Stories**  
  https://github.com/androso/artemus-atis/issues

### Laboratorio 1
- **Submitted Google Doc**  
  https://docs.google.com/document/d/1IFnn3Dr3zL77rxUA76MO5VupmA6fcenogtquvvH_Ngc/edit?usp=sharing

---

# 2. What the capstone is

The course calls the capstone the **Proyecto Integrador**.

It is intended to be a **semester-long team software-engineering project**. The course progressively adds artifacts to the same project:

1. project conception / RUP,
2. agile planning / Sprint 0,
3. Scrum organization,
4. backlog and user stories,
5. UML modeling,
6. later architecture, configuration, quality, and other engineering artifacts as the course advances.

The instructor's project **ReservaYA** is a teaching/reference example. It is not the team's capstone.

The team's current capstone is **Artemus App**.

---

# 3. Current Artemus product definition

The current GitHub project describes **Artemus App** as an interactive web application for **residential 2D layout generation**.

The intended flow is roughly:

1. a property owner enters terrain dimensions,
2. defines required rooms/spaces,
3. records architectural preferences,
4. the system generates a conceptual 2D residential layout,
5. the user can edit/regenerate alternatives,
6. the user formally accepts a version,
7. accepted layouts can be exported to PDF/DXF,
8. an architect can perform a formal technical review.

The current product therefore combines:

- requirements capture,
- terrain constraints,
- architectural program / room requirements,
- automatic 2D layout generation,
- interactive layout editing,
- versioning,
- acceptance workflow,
- technical export,
- architect review.

---

# 4. Important project evolution

The project changed substantially during the course.

## 4.1 Initial team formation — 17 July 2026

The submitted file:

`Equipo Artemus Tecnicas de Ingenieria.pdf`

states:

- **Team name:** Artemus
- **Members at that moment:**
  - Anibal Josue Campos Andrade
  - Elmer Stanley Garcia Amaya
  - Isaac Natanael Medrano Romero
  - Anderson Amilcar Fuentes Portillo
- **Coordinator:** Anibal Josué Campos Andrade
- **Initial project idea:**  
  > Automatización de call centers con inteligencia artificial para reducir los costos operativos de call centers modernos.

This is important because **the original Artemus idea was not the current residential-layout product**.

## 4.2 By Laboratorio 1

The Canvas screenshot for the submitted Google Doc shows:

- document title: **`Artemus App tecnicas`**
- the document is organized around **Fase de concepción (RUP)**
- a fifth member appears:
  - **Steisy Gissel Benítez Machado**

Visible outline items include:

- Documento de Visión
- Planteamiento del problema
- Objetivos del proyecto
- Objetivo general
- Objetivos específicos
- Alcance del proyecto
- Stakeholders
- Beneficios esperados

The full Google Doc could not be extracted in this run, so anything beyond the visible screenshot and course requirements should not be assumed.

## 4.3 By Laboratorio 2

The project is explicitly defined as:

> **Artemus App: aplicación web para generar propuestas conceptuales 2D de distribución de viviendas a partir de terreno, programa de espacios y preferencias, con exportación técnica y revisión por arquitecto.**

At this point:

- the team has **5 members**,
- the product is residential/architectural,
- a GitHub repository exists,
- a GitHub Projects board exists,
- there are 10 user stories,
- the team has a Sprint 0 and Definition of Done.

So somewhere between the initial team submission and the later labs, the project evolved from **AI call-center automation** into **residential 2D architectural layout generation**.

---

# 5. Team evolution

## Original team — Distribución de Equipos

| Member | Initial role/status |
|---|---|
| Aníbal Campos | Coordinator |
| Elmer Garcia | Team member |
| Isaac Medrano | Team member |
| Anderson Fuentes | Team member |

Initial team size: **4**

## Team shown by Laboratorio 1 / Laboratorio 2

| Member |
|---|
| Steisy Benítez |
| Aníbal Campos |
| Anderson Fuentes |
| Elmer Garcia |
| Isaac Medrano |

Later team size: **5**

This differs from the Session 01 course instruction saying teams should have four fixed members.

---

# 6. Actual capstone deliverables confirmed so far

This section treats a “step” as a **real deliverable/file/submission**, not as an individual section inside another document.

## Step 1 — Distribución de Equipos

**Canvas assignment ID:** `12972`  
**Submitted:** 2026-07-17 11:21 AM El Salvador time  
**Submission type:** online upload  
**File:** `Equipo Artemus Tecnicas de Ingenieria.pdf`  
**Grade recorded:** 1  
**Late:** No

Contains:

- team name,
- team members,
- coordinator,
- preliminary project idea.

Historical importance: this is the earliest artifact and preserves the **original call-center project idea**.

Canvas URL pattern:
https://univo.instructure.com/courses/1760/assignments/12972

---

## Step 2 — Laboratorio 1 — Documento de Concepción

**Canvas assignment ID:** `14830`  
**Submitted:** 2026-08-25 10:19 PM El Salvador time  
**Submission type:** online URL  
**Grade:** **77**  
**Late:** No

Submitted Google Doc:
https://docs.google.com/document/d/1IFnn3Dr3zL77rxUA76MO5VupmA6fcenogtquvvH_Ngc/edit?usp=sharing

Canvas export also contains an automatic screenshot:
`websnappr20260826-3687296-uew8j5.png`

### Course-required conception content

Across Sessions 02-05, Laboratorio 1 is built from:

- problem statement,
- general objective,
- specific objectives,
- project scope,
- stakeholders,
- project risks / risk matrix,
- business/process model or flow diagram.

These should be treated as **parts of the same Laboratorio 1 deliverable**, not separate deliverables.

Canvas:
https://univo.instructure.com/courses/1760/assignments/14830

---

## Step 3 — Laboratorio 2 — Plan de Proyecto Ágil / Sprint 0

**Canvas assignment ID:** `15429`  
**Submitted:** 2026-09-06 12:01 PM El Salvador time  
**Submission type:** online upload  
**File:** `Artemus-Lab2-Sprint0.pdf`  
**Grade:** **97**  
**Canvas marks submission as:** late

Canvas:
https://univo.instructure.com/courses/1760/assignments/15429

This is the major bridge between **project conception** and **technical/system modeling**.

It contains:

- project purpose,
- Scrum roles,
- GitHub Projects board,
- Product Backlog,
- priorities,
- Story Points,
- Sprint assignments,
- user stories,
- acceptance criteria,
- Definition of Done.

---

## Step 4 — Laboratorio 3 — Modelado UML del Proyecto Integrador

**Canvas assignment ID:** `17236`

The Canvas export dated 2026-09-28 shows **no submission from Aníbal's account**.

Course materials leading into Lab 3 include:

- class diagrams,
- sequence diagrams,
- activity diagrams.

The actual Lab 3 file may have been/will be submitted by another team member, so it is a priority file to retrieve.

Canvas:
https://univo.instructure.com/courses/1760/assignments/17236

---

# 7. Other team assignments that may be related to the capstone

These were **not submitted from Aníbal's Canvas account** according to the export. They may have been submitted by teammates.

## Práctica 01 — Fase de Concepción RUP y riesgos

**Assignment ID:** `15583`  
**Known due date from Notion/Canvas:** 2026-09-03 23:59 El Salvador

Expected as **one Word/PDF uploaded by one team member**, containing:

- cover,
- project plan,
- scope and justification,
- at least 4 risks,
- business-process diagram.

Important nuance: the course material frames this around a **POS + inventory system adapted to a selected business category**. It may be a controlled practice rather than a direct Artemus artifact. Do not merge it into the Artemus canon until the teammate file confirms it.

Canvas:
https://univo.instructure.com/courses/1760/assignments/15583

---

## Práctica 02 — Plan de Proyecto Ágil y Backlog

**Assignment ID:** `16013`  
**Known due date:** 2026-09-10 23:59 El Salvador

Expected as **one PDF uploaded by one member**, containing:

- Scrum roles,
- at least 8 user stories,
- acceptance criteria,
- agile/Kanban board screenshot.

The Notion course page explicitly connects this practice to the **Product Backlog inicial del proyecto integrador (Sprint 0)**, but it also uses “rubro” language. Retrieve the teammate file before deciding whether it is identical to / separate from Artemus Lab 2 work.

Canvas:
https://univo.instructure.com/courses/1760/assignments/16013

---

## Taller Integrador 18-09-2026

**Assignment ID:** `16752`  
**Status in Aníbal export:** no submission from Aníbal

There is currently no matching detailed page in the ATIS Notion Notes database, so its exact contents cannot be safely reconstructed from the stored course notes.

This is a **high-priority teammate file to retrieve** because of its date and its “Integrador” name.

Canvas:
https://univo.instructure.com/courses/1760/assignments/16752

---

## Práctica 03

**Assignment ID:** `17198`  
**Status in Aníbal export:** no submission from Aníbal

The Notion Notes database currently does not contain enough material to identify its exact contents.

This is another **high-priority teammate file to retrieve**.

Canvas:
https://univo.instructure.com/courses/1760/assignments/17198

---

# 8. September 26 class activity — not currently part of the Artemus capstone

Provided file:

`Actividad 1 Del enunciado al diagrama de clases.pdf`

The document is titled:

**Actividad 1: Del enunciado al diagrama de clases**

Case:

**Biblioteca universitaria**

It models:

- `Libro`
- `Estudiante`
- `Prestamo`

and includes:

- identification of classes/attributes,
- methods,
- multiplicities,
- UML class diagram,
- justification of modeling decisions.

This is useful **course/UML evidence**, but it uses a separate university-library case rather than Artemus.

Therefore it should currently be classified as:

> **ATIS coursework relevant to UML skills, but not an Artemus capstone deliverable.**

Canvas assignment ID from the export: `17179`.

---

# 9. Laboratorio 2 — exact submitted snapshot

The following reflects the **submitted PDF**, not later GitHub edits.

## 9.1 Cover / identity

Course:
**Aplicación de Técnicas de Ingeniería de Software**

Activity:
**Laboratorio 2 Plan de Proyecto Ágil (Sprint 0)**

Students:

- Benítez Machado, Steisy Gissel
- Campos Andrade, Aníbal Josué
- Fuentes Portillo, Anderson Amilcar
- Garcia Amaya, Elmer Estanley
- Medrano Romero, Isaac Natanael

Board:
https://github.com/users/androso/projects/9

Repo:
https://github.com/androso/artemus-atis

Document date:
**Friday, 4 September 2026 — San Miguel, El Salvador**

---

## 9.2 Purpose in submitted Lab 2

The PDF defines the project as:

> Artemus App: aplicación web para generar propuestas conceptuales 2D de distribución de viviendas a partir de terreno, programa de espacios y preferencias, con exportación técnica y revisión por arquitecto.

It says the document includes:

- initial Product Backlog,
- prioritization and estimation,
- Definition of Done,
- Scrum roles,
- link to the digital board.

---

## 9.3 Scrum roles in the submitted PDF

| Role | Person | Submitted-Lab-2 rationale |
|---|---|---|
| Product Owner | Steisy Benítez | Defines product vision and prioritizes backlog; business-requirement / stakeholder affinity |
| Scrum Master | **Aníbal Campos** | Facilitates agile process, removes impediments, cares for ceremonies/board; team organization |
| Development Team | Anderson Fuentes | Full-stack/mobile strengths |
| Development Team | Elmer Garcia | Technical deliverables and output quality |
| Development Team | Isaac Medrano | Review flows and data coherence |

This historical role assignment differs from the **current GitHub README**.

---

## 9.4 Submitted board configuration

Tool:
**GitHub Projects**

Board:
https://github.com/users/androso/projects/9

Repository:
https://github.com/androso/artemus-atis

Workflow columns:

1. Backlog
2. En progreso
3. En revisión
4. Hecho

Each story is represented as a GitHub issue/card with visible priority and Story Points.

---

# 10. Submitted Product Backlog

The submitted Lab 2 PDF reports:

- **10 user stories**
- **56 total Story Points**
- Planning Poker scale: **1, 2, 3, 5, 8**

## US-01 — Registro e inicio de sesión

**Actor:** propietario o arquitecto  
**Priority:** Alta  
**SP:** 5  
**Responsible:** Equipo (base)  
**Sprint:** Sprint 0

Story:

> Como propietario o arquitecto, quiero registrarme e iniciar sesión con correo electrónico y contraseña para acceder a mis proyectos y funcionalidades según mi rol en el sistema.

Acceptance criteria:

1. Incorrect credentials show “Credenciales inválidas” and deny access.
2. Successful login redirects according to role.
3. Email format and minimum password rules are validated.
4. Session uses a JWT and expires after inactivity / logout.

Current issue:
https://github.com/androso/artemus-atis/issues/1

---

## US-02 — Registrar terreno del proyecto

**Actor:** propietario  
**Priority:** Alta  
**SP:** 5  
**Responsible in submitted PDF:** Steisy Benítez  
**Sprint:** Sprint 0

Story:

> Como propietario, quiero ingresar frente, fondo, área total y orientación cardinal del terreno para que la propuesta arquitectónica conceptual se adapte a las dimensiones físicas reales.

Acceptance criteria:

1. Reject non-positive terrain dimensions.
2. Warn about inconsistency between total area and front × depth.
3. Require cardinal orientation.
4. Persist terrain and connect it to the active project / requirements summary.

Issue:
https://github.com/androso/artemus-atis/issues/2

---

## US-03 — Definir espacios y habitaciones

**Actor:** propietario  
**Priority:** Alta  
**SP:** 8  
**Responsible in submitted PDF:** Anderson Fuentes  
**Sprint:** Sprint 0

Story:

> Como propietario, quiero indicar los espacios requeridos con tipo, cantidad y área deseada para comunicar mis necesidades funcionales y de distribución del hogar.

Acceptance criteria:

1. Select spaces by zone or create a custom space.
2. Add/edit/delete spaces before generation.
3. Warn if requested area exceeds buildable area.
4. Enforce minimum habitable area rules.

Issue:
https://github.com/androso/artemus-atis/issues/3

---

## US-04 — Capturar preferencias de vivienda

**Actor:** propietario  
**Priority:** Alta  
**SP:** 3  
**Responsible in submitted PDF:** Anderson Fuentes  
**Sprint:** Sprint 0

Story:

> Como propietario, quiero registrar estilo, número de plantas, estacionamiento y previsión de ampliación para orientar la generación del layout según mis expectativas de vida y crecimiento.

Acceptance criteria:

1. Require number of floors and parking-space values.
2. Allow architectural style and future-expansion preference.
3. For multi-floor homes, allow preferred room distribution by level.
4. Persist preferences in technical/requirements summary.

Issue:
https://github.com/androso/artemus-atis/issues/4

---

## US-05 — Generar propuesta conceptual 2D

**Actor:** propietario  
**Priority:** Alta  
**SP in submitted PDF:** **8**  
**Responsible in submitted PDF:** **Anderson Fuentes**  
**Sprint in submitted PDF:** **Sprint 0**

Story:

> Como propietario, quiero generar una distribución conceptual 2D a partir del terreno, espacios y preferencias para visualizar una alternativa arquitectónica funcional y clara de mi vivienda.

Acceptance criteria:

1. Validate required terrain + minimum room data before calculation.
2. Place rooms without overlaps and respect terrain/setback constraints.
3. Render a 2D canvas with labels/areas and version the layout.
4. Show requested area vs obtained area.

Issue:
https://github.com/androso/artemus-atis/issues/5

---

## US-06 — Editar y regenerar el layout

**Actor:** propietario  
**Priority:** Media  
**SP:** 8  
**Responsible in submitted PDF:** **Anderson Fuentes**  
**Sprint:** Backlog

Story:

> Como propietario, quiero ajustar posición/dimensiones de habitaciones o regenerar una alternativa para acercar el diseño a mis necesidades particulares antes de aceptarlo formalmente.

Acceptance criteria:

1. Interactive repositioning with collision/boundary checks.
2. Every edit/regeneration produces a new sequential version.
3. Previous versions can be navigated and restored.

Issue:
https://github.com/androso/artemus-atis/issues/6

---

## US-07 — Aceptar propuesta conceptual

**Actor:** propietario  
**Priority:** Alta  
**SP:** 3  
**Responsible:** Elmer Garcia  
**Sprint:** Backlog

Acceptance criteria:

1. Only valid/conflict-free versions can be accepted.
2. Accepted proposal becomes read-only / pending review.
3. Explicit confirmation before acceptance.
4. Acceptance enables PDF/DXF export and architect review.

Issue:
https://github.com/androso/artemus-atis/issues/7

---

## US-08 — Exportar a PDF y DXF

**Actor:** propietario o arquitecto  
**Priority:** Alta  
**SP:** 8  
**Responsible:** Elmer Garcia  
**Sprint:** Backlog

Acceptance criteria:

1. PDF contains cover, requirements summary and dimensioned 2D plan.
2. DXF uses normalized layers and metric 1:1 scale.
3. Export uses standardized naming and opens in common PDF/CAD tools.

Issue:
https://github.com/androso/artemus-atis/issues/8

---

## US-09 — Revisión por arquitecto

**Actor:** arquitecto  
**Priority:** Media  
**SP:** 5  
**Responsible:** Isaac Medrano  
**Sprint:** Backlog

Acceptance criteria:

1. Architect can view accepted plan and complete project inputs.
2. Decision is either “Aprobado” or “Requiere Ajustes”.
3. “Requiere Ajustes” requires technical comments.
4. Decision is audited with date/time/architect and user notification.

Issue:
https://github.com/androso/artemus-atis/issues/9

---

## US-10 — Resumen de requisitos del proyecto

**Actor:** propietario o arquitecto  
**Priority:** Media  
**SP:** 3  
**Responsible:** Isaac Medrano  
**Sprint:** Sprint 0

Acceptance criteria:

1. Consolidate terrain, spaces and preferences.
2. Highlight missing/inconsistent information.
3. Provide direct edit navigation for each block.

Issue:
https://github.com/androso/artemus-atis/issues/10

---

# 11. Sprint 0 according to the submitted Lab 2 PDF

Submitted Sprint 0 stories:

- US-01 — 5 SP
- US-02 — 5 SP
- US-03 — 8 SP
- US-04 — 3 SP
- US-05 — 8 SP
- US-10 — 3 SP

Total from these values:
**32 SP**

The submitted PDF labels US-06 through US-09 as Backlog.

---

# 12. Definition of Done — submitted Lab 2 version

The submitted PDF defines a story as done only when:

1. all acceptance criteria have been manually verified in the Artemus UI/API;
2. layout-related work has no spatial collisions or failed terrain/space validations;
3. there is a Pull Request reviewed/approved by at least one Development Team peer;
4. the GitHub issue is updated with status, priority, SP and PR link;
5. if project data changes, the requirements summary correctly reflects it without unjustified critical warnings;
6. compiling is not enough — the item must be demonstrable on the board with evidence such as screenshot/checklist in the PR.

This is the **historical DoD that appears in the submitted PDF**.

---

# 13. Current GitHub state

The GitHub repository has evolved after / apart from the submitted PDF.

## Repository metadata

Repository:
https://github.com/androso/artemus-atis

- public repository
- default branch: `main`

Known commits from the connected GitHub source:

1. **Initial commit: Artemus App README and ATIS team**  
   2026-09-03
2. **docs: add full Laboratorio 2 Sprint 0 planning, DoD, and user stories**  
   2026-09-03

---

## Current roles in README

The current README says:

| Person | Current README role | Stories |
|---|---|---|
| Steisy Benítez | Product Owner | US-01, US-02 |
| **Anderson Fuentes** | **Scrum Master** | US-03, US-04 |
| **Aníbal Campos** | **Developer** | US-05, US-06 |
| Elmer Garcia | Developer | US-07, US-08 |
| Isaac Medrano | Developer | US-09, US-10 |

This differs from the submitted PDF, where **Aníbal was Scrum Master** and **Anderson was Development Team**.

---

## Current Sprint Goal in README

> “Establecer la infraestructura base, arquitectura del sistema, entorno de desarrollo y la implementación del núcleo de captura de requisitos residenciales (autenticación segura, dimensiones del terreno, programa de espacios y preferencias arquitectónicas), dejando el backlog priorizado, estimado y validado para la generación del layout 2D.”

---

## Current README Definition of Done

The current README uses a more software-delivery-oriented DoD:

1. acceptance criteria verified,
2. code style/linter/compilation standards,
3. automated unit/integration tests with at least 80% coverage on affected modules,
4. Pull Request with independent technical approval,
5. technical documentation and updated issue,
6. deployed and working in a staging/test environment without regressions.

This is **not identical** to the DoD in the submitted Lab 2 PDF.

---

# 14. Current GitHub issues — operational backlog

The current GitHub issues report:

| ID | Story | Current issue responsible | Priority | SP | Sprint |
|---|---|---|---|---:|---|
| US-01 | Registro e inicio de sesión | Equipo (base) | Alta | 5 | Sprint 0 |
| US-02 | Registrar terreno del proyecto | Steisy Benítez (PO) | Alta | 5 | Sprint 0 |
| US-03 | Definir espacios y habitaciones | Anderson Fuentes (SM) | Alta | 8 | Sprint 0 |
| US-04 | Capturar preferencias de vivienda | Anderson Fuentes (SM) | Alta | 3 | Sprint 0 |
| US-05 | Generar propuesta conceptual 2D | **Aníbal Campos (Dev)** | Alta | **8** | **Sprint 0** |
| US-06 | Editar y regenerar el layout | **Aníbal Campos (Dev)** | Media | 8 | Backlog |
| US-07 | Aceptar propuesta conceptual | Elmer Garcia (Dev) | Alta | 3 | Backlog |
| US-08 | Exportar a PDF y DXF | Elmer Garcia (Dev) | Alta | 8 | Backlog |
| US-09 | Revisión por arquitecto | Isaac Medrano (Dev) | Media | 5 | Backlog |
| US-10 | Resumen de requisitos del proyecto | Isaac Medrano (Dev) | Media | 3 | Sprint 0 |

This issue-level state is currently the cleanest operational mapping of ownership.

---

# 15. GitHub drift / inconsistencies to be aware of

There are meaningful differences between:

- the **submitted Lab 2 PDF**,
- the **current GitHub README**,
- the **current GitHub issues**.

Do not silently merge them.

## 15.1 Scrum Master

**Submitted PDF:**
- Scrum Master = **Aníbal Campos**

**Current README/issues:**
- Scrum Master = **Anderson Fuentes**
- Aníbal = Developer

---

## 15.2 US-05 ownership

**Submitted PDF:**
- US-05 responsible = **Anderson Fuentes**

**Current README/issues:**
- US-05 responsible = **Aníbal Campos**

---

## 15.3 US-05 Story Points / sprint placement

**Submitted PDF:**
- 8 SP
- Sprint 0

**Current issue #5:**
- 8 SP
- Sprint 0

**Current README:**
- **13 SP**
- **Backlog**
- README Sprint 0 section omits US-05.

Thus the current README is not synchronized with issue #5 or the submitted Lab 2 PDF.

---

## 15.4 Total backlog points

**Submitted PDF:** reports **56 SP**

The current issues sum to:

5 + 5 + 8 + 3 + 8 + 8 + 3 + 8 + 5 + 3 = **56 SP**

The current README says:

- **58 SP** total for 10 stories
- **50 SP** for the eight base stories

but its visible story table also assigns US-05 = 13 SP, which causes another arithmetic mismatch.

The **current issue values and submitted PDF both support 56 SP**.

---

## 15.5 Sprint 0 total

Submitted PDF / current issue state includes:

US-01 + US-02 + US-03 + US-04 + US-05 + US-10

= 5 + 5 + 8 + 3 + 8 + 3  
= **32 SP**

Current README states **24 SP** and uses:

US-01 + US-02 + US-03 + US-04 + US-10

The difference is entirely US-05.

---

## 15.6 Definition of Done

The submitted PDF has a project-specific verification/evidence DoD.

The current README has a stricter engineering DoD involving:

- linter/build,
- automated tests,
- coverage,
- code review,
- docs,
- staging deployment.

This may represent a later refinement rather than what was actually submitted.

---

# 16. Course-material roadmap as it relates to the capstone

The ATIS Notes database currently contains **16 pages**.

## Session 01 — 17/07/2026 — Presentación del curso y diagnóstico

Relevant project requirements:

- semester-long Proyecto Integrador,
- team formation,
- preliminary idea,
- project documentation grows across units,
- ReservaYA is only the guide/example,
- all team members should contribute.

Notion:
https://app.notion.com/p/3a082a6d6561806da420e077b2e27f2f

---

## Session 02 — 18/07/2026 — Fase de concepción RUP y documento de visión

Feeds Laboratorio 1.

Team works on:

- problem,
- objective general,
- specific objectives,
- scope,
- stakeholders.

Notion:
https://app.notion.com/p/3a382a6d6561805988a2cdc4b2c8ee23

---

## Session 03 — 24/07/2026 — Matriz de riesgos del proyecto

Feeds Laboratorio 1.

Team identifies project risks by:

- category,
- probability,
- impact,
- mitigation.

Notion:
https://app.notion.com/p/3aa82a6d6561810c82d6db1cb7062342

---

## Session 04 — 25/07/2026 — Diagrama del modelo de negocio

Feeds Laboratorio 1.

Project work:

- actors,
- process steps,
- decisions,
- alternative paths,
- outcomes,
- diagram through Mermaid or draw.io.

Notion:
https://app.notion.com/p/3aa82a6d656181449560e35755047028

---

## Session 05 — 31/07/2026 — Revisión y entrega del Laboratorio 1

Consolidates the conception work into the Lab 1 document.

Notion:
https://app.notion.com/p/3c482a6d656181bba879fa9207cb3ba0

---

## Session 06 — 01/08/2026 — Manifiesto Ágil, Scrum y Kanban

Project teams analyze:

- Scrum,
- Kanban,
- predictive,
- hybrid approaches.

The activity product is described as a **ficha de análisis + explicación oral**.

No separate confirmed capstone Canvas deliverable has been established from the available export.

Notion:
https://app.notion.com/p/3c482a6d6561814c8f5fed5386d23df4

---

## Session 07 — 14/08/2026 — Sprint, Backlog y GitHub Projects

Directly feeds **Laboratorio 2**.

Required project work includes:

- Product Backlog,
- Sprint Backlog,
- GitHub Projects board,
- priorities,
- estimates,
- Sprint 0,
- Sprint objective,
- Definition of Done,
- responsibilities.

Notion:
https://app.notion.com/p/3c482a6d656181c69e55e67cef2de47a

---

## Session 08 — 15/08/2026 — Historias de usuario y estimación ágil

Project work:

- user stories,
- actor / need / benefit,
- acceptance criteria,
- Planning Poker,
- priorities,
- points,
- Definition of Done,
- updated backlog.

Expected evidence for the original team-of-four framing:

- 8 stories,
- at least 3 acceptance criteria per story,
- priority,
- points,
- DoD,
- updated GitHub Projects backlog.

Notion:
https://app.notion.com/p/3c982a6d656181158022ddaf0dea3621

---

## Session 09 — 21/08/2026 — Roles y eventos en Scrum

Project work:

- assign PO / SM / Developers,
- define functions,
- simulate Daily Scrum.

Important:
the Notion page explicitly says **there is no Canvas assignment submission for this session**.

Notion:
https://app.notion.com/p/3cd82a6d6561812d90b9ff33232af6ae

---

## Session 10 — 22/08/2026 — Taller integrador: consolidación del Sprint 0

Teams review:

- conception document,
- Product Backlog,
- stories,
- criteria,
- priority,
- estimates,
- roles,
- DoD,
- board.

Includes peer review.

Important:
the page explicitly states this is **not a new Laboratorio 2 submission**; it is a refinement/update of the existing material.

Notion:
https://app.notion.com/p/3c882a6d656181db9b96e4591a963b98

---

## Práctica 01 — 21/08/2026 — Fase de Concepción RUP y riesgos

Separate Canvas deliverable, one team file.

Potentially related, but course material uses a POS/inventory case.

Notion:
https://app.notion.com/p/3cd82a6d65618119956ae81c2534ee15

---

## Práctica 02 — 28/08/2026 — Plan de Proyecto Ágil y Backlog

Separate team PDF.

Explicitly references initial Product Backlog / Sprint 0.

Notion:
https://app.notion.com/p/3d182a6d6561819098b8e19940f8e7d2

---

## Session 11 — 28/08/2026 — Primer Examen Parcial

Individual evaluation of:

- RUP conception,
- agile fundamentals.

Not a capstone deliverable, but it marks the end of the first conceptual/agile block.

Notion:
https://app.notion.com/p/3d982a6d6561818688fae807160eb313

---

## Session 13 — 04/09/2026 — Introducción al modelado UML

Begins Unit 3.

Each team starts deciding which structural/behavioral diagrams are appropriate for its Proyecto Integrador.

Notion:
https://app.notion.com/p/3e082a6d656181e4ad50ceec466d4fa4

---

## Session 14 — 05/09/2026 — Diagrama de clases

Each team begins the **class diagram for its Proyecto Integrador**.

This is explicitly described as progress toward **Laboratorio 3**.

Notion:
https://app.notion.com/p/3e082a6d656181069c91f12445e22c1c

---

## Session 15 — 11/09/2026 — Diagramas de secuencia y actividad

Each team should develop:

- sequence diagram,
- activity diagram,

for one functionality of the Proyecto Integrador.

This is also explicitly identified as progress toward **Laboratorio 3**.

Notion:
https://app.notion.com/p/3e782a6d6561812c8269d3b7e7850e7a

---

# 17. Current course stage

Based on the **latest course material currently stored in Notion**, the capstone has entered the:

> **UML modeling phase / preparation for Laboratorio 3**

The course-material sequence is:

**Conception → Sprint 0 / agile planning → UML modeling**

Specifically:

**Lab 1**  
defines what the system is, the problem, scope and stakeholders.

**Lab 2 / Sprint 0**  
turns the concept into backlog, stories, estimates, responsibilities and a working project board.

**Lab 3**  
models the same system structurally and behaviorally using UML.

---

# 18. Important freshness gap in Notion

The course Notes database currently stops at:

**Session 15 — 11/09/2026**

However, the Canvas submission export shows later assignments such as:

- Taller Integrador 18-09-2026
- Actividad 1: Del enunciado al diagrama de clases
- Práctica 03
- Laboratorio 3

Therefore:

> **The Notion course notes are not complete for the period after September 11.**

Do not assume the Notion Notes database alone represents the latest Canvas requirements.

---

# 19. Canvas submission snapshot — 28 September 2026

The exported Canvas manifest says Aníbal had submissions for **6 of 13 assignments**.

## Submitted from Aníbal's account

| Assignment | ID | Relevant to capstone? | Result |
|---|---:|---|---|
| Prueba Diagnostica | 12281 | No/directly no | 6/20 |
| Roll Call Attendance | 12969 | No | 100% |
| **Distribución de Equipos** | **12972** | **Yes** | submitted |
| **Entrega del Primer Laboratorio** | **14830** | **Yes** | **77** |
| **Entrega del segundo Laboratorio** | **15429** | **Yes** | **97** |
| Primer Examen Parcial | 16399 | Course knowledge, not capstone file | ~96.36 |

## Not submitted from Aníbal's account

| Assignment | ID | Current interpretation |
|---|---:|---|
| Práctica 01 | 15583 | teammate file needed; possibly related |
| Práctica 02 | 16013 | teammate file needed; likely related to Sprint 0 |
| Taller Integrador 18-09-2026 | 16752 | teammate file needed; likely relevant |
| Diferido de parcial | 16814 | not relevant unless taken |
| Actividad 1: Del enunciado al diagrama de clases | 17179 | separate Biblioteca case; file now available |
| Práctica 03 | 17198 | teammate file needed |
| **Laboratorio 3: Modelado UML del Proyecto Integrador** | **17236** | **core capstone file needed** |

Important:
“not submitted from Aníbal's account” **does not mean the team failed to submit it**. A teammate may have submitted the group assignment.

---

# 20. Recommended file-recovery priority

When gathering files from teammates, search in this order:

1. **Laboratorio 3 — Modelado UML del Proyecto Integrador**
2. **Taller Integrador 18-09-2026**
3. **Práctica 03**
4. **Práctica 02**
5. **Práctica 01**

Then verify whether each file actually uses **Artemus** before adding it to the canonical capstone history.

---

# 21. What should currently be considered canonical

Because the project evolved and sources conflict, use this hierarchy depending on the question.

## “What did we actually turn in?”

Use:

1. submitted PDFs / Google Doc,
2. Canvas export metadata.

For Lab 2, the file `Artemus-Lab2-Sprint0.pdf` is the best historical source.

## “What is the current backlog / ownership?”

Use:

1. GitHub issues,
2. GitHub Projects board.

Issues currently have the most internally coherent 56-SP backlog.

## “What does the course expect?”

Use:

1. Notion course session pages,
2. Canvas assignment instructions when available.

## “What is our current capstone summary?”

Use the Notion page:

**Proyecto Integrador — Artemus App**  
https://app.notion.com/p/3e982a6d656181f5a032c82bea7bb0e2

---

# 22. Open questions / unresolved items

These should not be silently guessed.

1. **When exactly did the project change from AI call centers to residential 2D architecture?**
   - The initial team file has the call-center idea.
   - Later labs clearly use the residential product.
   - The exact decision point is not yet documented.

2. **Why was Steisy added as a fifth member?**
   - She is absent from the initial team PDF.
   - She is present by Lab 1 / Lab 2.
   - Course Session 01 originally said four fixed members.

3. **What is the official current Scrum Master assignment?**
   - Submitted PDF: Aníbal.
   - Current GitHub: Anderson.

4. **Is US-05 currently 8 or 13 SP?**
   - Submitted PDF: 8.
   - Current issue #5: 8.
   - Current README: 13.

5. **Is US-05 in Sprint 0 or Backlog?**
   - Submitted PDF: Sprint 0.
   - Current issue #5: Sprint 0.
   - Current README: Backlog.

6. **Which DoD is official?**
   - Submitted Lab 2 version and current README version differ.

7. **What exactly was submitted for Práctica 01, Práctica 02, Taller Integrador, Práctica 03 and Lab 3?**
   - Files from teammates are still needed.

8. **What is in the full Laboratorio 1 Google Doc?**
   - The link and screenshot exist, but the full Google Doc text was not accessible during this consolidation.

9. **What course material came after Session 15?**
   - Canvas clearly has later assignments, but the Notion Study Journal has not yet captured those later class pages.

---

# 23. Source inventory

## Local / submitted files

From `ats-submitted-homeworks.zip`:

- `Distribución-de-Equipos/Equipo Artemus Tecnicas de Ingenieria.pdf`
- `Entrega-del-Primer-Laboratorio/submitted-url.txt`
- `Entrega-del-Primer-Laboratorio/websnappr20260826-3687296-uew8j5.png`
- `Entrega-del-segundo-Laboratorio/Artemus-Lab2-Sprint0.pdf`
- `MANIFEST.md`

Additional conversation attachment:

- `Actividad 1 Del enunciado al diagrama de clases.pdf`

## Notion

Course:
https://app.notion.com/p/a748067844f942cb959b723986eef896

Capstone page:
https://app.notion.com/p/3e982a6d656181f5a032c82bea7bb0e2

## GitHub

Repository:
https://github.com/androso/artemus-atis

Project:
https://github.com/users/androso/projects/9

Issues:
https://github.com/androso/artemus-atis/issues

---

# 24. Short project timeline

```text
17 Jul
Team "Artemus" formed
4 members
Aníbal coordinator
Initial idea = AI call-center automation
        |
        v
Jul-Aug
RUP conception work
vision -> risks -> business/process modeling
        |
        v
25 Aug
Lab 1 submitted
"Artemus App tecnicas"
5-person team visible
        |
        v
3 Sep
GitHub repo / Lab 2 docs created
        |
        v
6 Sep
Lab 2 submitted
Residential 2D-layout product firmly defined
GitHub Project + backlog + Sprint 0 + DoD
        |
        v
Sep
UML unit begins
class / sequence / activity diagrams
        |
        v
18-28 Sep
Later Canvas assignments exist
Taller Integrador / Activity 1 / Practice 03 / Lab 3
Not all are represented in Notion
Teammate files still being gathered
```

---

# 25. One-sentence state of the project

> **Artemus began as a team name attached to an AI call-center idea, evolved into a five-person residential 2D-layout software project, completed its conception and Sprint 0 deliverables, is managed through `androso/artemus-atis` and GitHub Project #9, and is now in the UML/Laboratorio 3 stage, with several teammate-submitted artifacts still needing to be collected and reconciled.**
