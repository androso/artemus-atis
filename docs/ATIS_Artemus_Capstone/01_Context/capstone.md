# Proyecto Integrador ATIS: Artemus App (contexto para la Práctica 06)

Fuente: Notion, Study Journal > Aplicación de Técnicas de Ingeniería de Software > "Proyecto Integrador, Artemus App" (https://app.notion.com/p/3e982a6d656181f5a032c82bea7bb0e2), Laboratorio 2 entregado (Artemus_Lab2_Sprint0_entregable.pdf), Laboratorio 3 (modelo de clases) y repositorio github.com/androso/artemus-atis.

## Qué es
Artemus App es una aplicación web interactiva para el diseño conceptual de distribuciones residenciales en 2D. Funciona así:
1. El propietario ingresa las medidas del terreno.
2. Define los espacios que necesita.
3. Registra sus preferencias.
4. El sistema genera un layout 2D conceptual y sin solapes.
5. El propietario puede editarlo o regenerarlo (cada cambio crea una nueva versión).
6. Acepta formalmente una versión.
7. La exporta a PDF o DXF.
8. Un arquitecto la revisa (Aprobado o Requiere Ajustes).

Actores: Propietario, Arquitecto.

## Equipo
| Integrante | Rol Scrum (Lab 2 entregado) | Historias a cargo (issues de GitHub) | Carné |
|---|---|---|---|
| Steisy Gissel Benítez Machado | Product Owner | US-01, US-02 | [CARNÉ] |
| Anibal Josue Campos Andrade | Scrum Master (en el README actual: Developer) | US-05, US-06 | [CARNÉ] |
| Anderson Amilcar Fuentes Portillo | Development Team (en el README actual: Scrum Master) | US-03, US-04 | [CARNÉ] |
| Elmer Stanley Garcia Amaya | Development Team | US-07, US-08 | [CARNÉ] |
| Isaac Natanael Medrano Romero | Development Team | US-09, US-10 | [CARNÉ] |

## Product Backlog (Sprint 0, 10 HU, 56 SP)
- **US-01 Registro e inicio de sesión** (Alta, 5 SP). Como propietario o arquitecto, quiero registrarme e iniciar sesión con correo y contraseña para acceder a mis proyectos según mi rol. Criterios: credenciales incorrectas muestran "Credenciales inválidas"; redirección según rol; validación de formato de correo y contraseña mínima; sesión con JWT que expira a los 60 min de inactividad.
- **US-02 Registrar terreno** (Alta, 5 SP). Como propietario, quiero ingresar frente, fondo, área total y orientación cardinal del terreno para que la propuesta se adapte a las dimensiones reales. Criterios: rechaza medidas no positivas; advierte si el área total no cuadra con frente × fondo; orientación obligatoria; se guarda ligado al proyecto.
- **US-03 Definir espacios y habitaciones** (Alta, 8 SP). Como propietario, quiero indicar los espacios requeridos con tipo, cantidad y área deseada. Criterios: elegir por zona o crear espacio personalizado; agregar, editar y eliminar antes de generar; advertencia si el área pedida supera el área construible; área mínima habitable.
- **US-04 Capturar preferencias** (Alta, 3 SP). Estilo, número de plantas, estacionamientos y previsión de ampliación. Plantas y estacionamientos son obligatorios.
- **US-05 Generar propuesta conceptual 2D** (Alta, 8 SP, a cargo de Anibal en GitHub). Como propietario, quiero generar una distribución conceptual 2D a partir del terreno, espacios y preferencias para visualizar una alternativa arquitectónica funcional y clara de mi vivienda. Criterios:
  1. Validar el terreno y los datos mínimos de espacios antes de calcular.
  2. Ubicar los espacios sin solapes, respetando los límites y retiros del terreno.
  3. Mostrar un canvas 2D con etiquetas y áreas, y versionar el layout.
  4. Mostrar el área solicitada frente al área obtenida.
- **US-06 Editar y regenerar el layout** (Media, 8 SP). Mover y redimensionar con control de colisiones; cada cambio crea una versión secuencial; se puede volver a versiones previas.
- **US-07 Aceptar propuesta** (Alta, 3 SP). Solo versiones válidas; queda de solo lectura y pendiente de revisión; requiere confirmación.
- **US-08 Exportar a PDF y DXF** (Alta, 8 SP). PDF con portada, resumen y plano acotado; DXF con capas normalizadas a escala 1:1.
- **US-09 Revisión por arquitecto** (Media, 5 SP). Decisión "Aprobado" o "Requiere Ajustes" (con comentarios); auditoría con fecha y arquitecto.
- **US-10 Resumen de requisitos** (Media, 3 SP). Consolida terreno, espacios y preferencias; resalta faltantes e inconsistencias.

## Modelo de clases del dominio (Laboratorio 3)
- Usuario (id, nombre, correo, hashContrasena, rol)
- ProyectoVivienda (id, estado), con 1 Terreno, 0..* EspacioRequerido, 0..1 PreferenciasVivienda y 0..1 Propuesta
- Terreno (frente, fondo, areaTotal, orientacion)
- EspacioRequerido (tipo, cantidad, areaDeseada, zona)
- PreferenciasVivienda (estilo, numeroPlantas, estacionamientos, ampliacion)
- Propuesta (id, estado), con 1..* VersionLayout
- VersionLayout (numero, estado; valida solapes y límites)
- Exportacion (formato, nombreArchivo), RevisionArquitectonica (decision, comentario, fecha), ResumenRequisitos (faltantes, inconsistencias)

Flujo de US-05 según el Lab 3:
1. El propietario solicita la generación.
2. Se verifica que existan terreno, espacios y preferencias. Si falta algo, se indica qué completar.
3. Se calcula la distribución.
4. Se valida que no haya solapes, que todo esté dentro de los límites y que las áreas cuadren. Si algo falla, se ajusta.
5. Se crea la versión 1 y se muestran el canvas, las etiquetas y las áreas obtenidas.

## Tecnología
El capstone no fija un stack. Lo único documentado es que es una aplicación web con autenticación JWT y que el repositorio es github.com/androso/artemus-atis (hoy solo tiene documentación: README, backlog y DoD).
