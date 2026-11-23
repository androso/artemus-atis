# Prompt para ChatGPT: ATIS Práctica 06 (Arquitectura en Capas sobre Artemus App)

## Archivos que hay que subir a ChatGPT junto con este prompt
1. `/workspace/homework/atis/p06/raw/Guia_Practica_06_Arquitectura_Capas.pdf` (guía oficial, obligatoria).
2. `/workspace/homework/atis/p06/capstone.md` (contexto del Proyecto Integrador Artemus App: equipo, backlog y modelo de clases).

Antes de enviar, reemplaza los [CARNÉ] si ya tienes los números. Si no, quedarán como marcadores en la portada.

---

## Prompt (copiar desde aquí)

Necesito preparar la Práctica 06 de Aplicación de Técnicas de Ingeniería de Software (UNIVO): "Vista de Diseño: Arquitectura en Capas". Te adjunto dos archivos: la guía oficial de la Práctica 06 (PDF) y `capstone.md`, que tiene el contexto de nuestro Proyecto Integrador, Artemus App. Léelos completos antes de empezar. La guía define qué se entrega. El capstone define el sistema sobre el que se trabaja.

Punto clave: la guía usa como ejemplo un Punto de Venta, pero nuestro sistema es Artemus App, una aplicación web para generar distribuciones residenciales 2D. Todo el documento debe estar hecho sobre Artemus. Toma de la guía la estructura, las reglas y el nivel de detalle, pero cambia el contenido de venta, stock e IVA por el dominio de Artemus: terreno, espacios, preferencias, propuestas y versiones de layout. No menciones ventas, productos ni rubros comerciales.

Datos del equipo (para la portada):
- Steisy Gissel Benítez Machado, carné [CARNÉ]
- Anibal Josue Campos Andrade, carné [CARNÉ]
- Anderson Amilcar Fuentes Portillo, carné [CARNÉ]
- Elmer Stanley Garcia Amaya, carné [CARNÉ]
- Isaac Natanael Medrano Romero, carné [CARNÉ]
- Proyecto: Artemus App, diseño conceptual de viviendas en 2D (en el campo "rubro" de la portada pon: "Diseño arquitectónico residencial, Artemus App")
- Docente: Josué Exequiel Montoya Sánchez
- Fecha: 18 de octubre de 2026

Diseño que debe tener el documento (respeta estos nombres en todas las secciones):

Capa de presentación (`capa_presentacion`, estereotipo «view»), con una pantalla por historia del backlog:
- FrmLogin (US-01)
- FrmTerreno (US-02)
- FrmEspacios (US-03)
- FrmGeneradorLayout (US-05: botón Generar, canvas 2D, etiquetas y áreas)

Capa lógica (`capa_logica`, estereotipo «controller»), un controlador por pantalla:
- AuthController
- TerrenoController
- EspacioController
- PropuestaController

Las reglas de negocio viven aquí:
- validar medidas positivas y coherencia entre área y frente × fondo;
- área mínima habitable;
- que la suma de áreas no supere el área construible;
- ubicación sin solapes y dentro de los retiros;
- numeración de versiones.

Capa de datos (`capa_datos`, estereotipo «dao»):
- ConexionBD
- Un DAO por tabla:
  - UsuarioDAO (usuarios)
  - ProyectoDAO (proyectos)
  - TerrenoDAO (terrenos)
  - EspacioDAO (espacios_requeridos)
  - PreferenciasDAO (preferencias_vivienda)
  - PropuestaDAO (propuestas)
  - VersionLayoutDAO (versiones_layout)

Si ves que falta o sobra algo para que el diseño sea coherente, ajústalo y anótalo en Suposiciones.

Qué tienes que entregar:

Un archivo PDF descargable llamado `Practica06_Arquitectura_Capas_Equipo.pdf`, listo para subir a Canvas (el curso exige un único PDF). Debe estar en español y contener, en este orden:

1. Portada formal: Universidad de Oriente (UNIVO), materia, "Práctica 06: Vista de Diseño, Arquitectura en Capas", nombres completos con carné, proyecto y rubro, docente y fecha.
2. Componentes por capa: una tabla corta con cada clase, su capa y su responsabilidad en Artemus.
3. Diagrama de Paquetes UML como imagen nítida dentro del PDF:
   - los tres paquetes apilados de arriba hacia abajo;
   - cada clase con su estereotipo;
   - dependencias punteadas con la etiqueta «use», siempre hacia abajo (vista hacia controlador, controlador hacia DAO, DAO hacia ConexionBD);
   - ninguna flecha hacia arriba y ninguna vista conectada directo a un DAO.
4. Tabla de Mapeo de Carpetas con estas columnas: Paquete UML, Carpeta en GitHub, Archivos, Contenido. El repositorio es github.com/androso/artemus-atis. Usa `src/views/`, `src/controllers/` y `src/models/` con archivos .py en snake_case, como en la guía (frm_generador_layout.py, propuesta_controller.py, conexion.py, version_layout_dao.py, etc.). Agrega un árbol corto del repositorio.
5. Recorrido Técnico de la Transacción, aplicado a la historia **US-05 Generar propuesta conceptual 2D**: "Como propietario, quiero generar una distribución conceptual 2D a partir del terreno, espacios y preferencias para visualizar una alternativa arquitectónica funcional y clara de mi vivienda." Escríbelo en pasos numerados:
   - el clic en "Generar" en FrmGeneradorLayout y los datos que envía (proyecto_id);
   - la llamada a `PropuestaController.generar_propuesta(proyecto_id)`;
   - las lecturas que pide el controlador: TerrenoDAO, EspacioDAO y PreferenciasDAO, con sus SELECT;
   - las reglas que valida antes y durante el cálculo, siguiendo los criterios de aceptación de US-05;
   - la escritura en una sola transacción: INSERT en propuestas, INSERT de la versión 1 en versiones_layout (con área solicitada, área obtenida y la geometría) y UPDATE del estado en proyectos, cerrando con commit;
   - lo que se devuelve a la vista: canvas con etiquetas, comparación de áreas y el mensaje al usuario.
   Agrega también un caso de error, por ejemplo cuando las áreas pedidas superan el área construible: no se escribe nada (rollback) y la vista muestra qué debe corregir el usuario.
6. Justificación del desacoplamiento: un solo párrafo de 4 a 5 líneas, con nuestras palabras. Debe comparar esta arquitectura con poner SQL dentro de las pantallas y dar un ejemplo concreto de Artemus, como cambiar el algoritmo de generación o el motor de base de datos sin tocar FrmGeneradorLayout.

Reglas de la guía que no se pueden romper:
- nada de SQL ni cálculos de áreas o validaciones en la capa de presentación;
- las reglas de negocio solo en los controladores;
- el SQL solo en los DAO;
- las dependencias solo hacia abajo.

Diagrama en el chat: además de la imagen dentro del PDF, escribe aquí el código Mermaid del Diagrama de Paquetes. Usa `flowchart TB`, con un `subgraph` por paquete, el estereotipo dentro del texto de cada nodo y flechas punteadas `-.->|«use»|`, para poder editarlo en Mermaid Live o pasarlo a draw.io.

Estilo de redacción:
- Español claro de estudiantes universitarios de El Salvador; frases cortas y concretas.
- No uses guiones largos (— o –). Usa comas, dos puntos o paréntesis.
- No uses frases de relleno como "en el mundo actual", "es importante destacar", "cabe mencionar", "en conclusión", "juega un papel crucial" ni "robusto y escalable".
- No pongas introducciones ni conclusiones genéricas que la guía no pide. Cada sección va directo a su contenido.
- Nada de emojis, negritas en exceso, cajas decorativas ni plantillas llamativas. Formato sobrio: títulos numerados, tablas simples, Calibri o Arial 11, márgenes normales.
- Los mismos nombres de clases, métodos y tablas en el diagrama, la tabla de mapeo y el recorrido.

Al final de tu respuesta en el chat, después del enlace al PDF y del código Mermaid, agrega una lista llamada "Suposiciones" con un máximo de 6 puntos. Incluye como mínimo:
- que se adaptó el ejemplo de Punto de Venta de la guía al dominio de Artemus App;
- que la traza usa US-05 del backlog del capstone, porque la guía pide la historia de la Práctica 05;
- el stack y el motor de base de datos que asumiste, porque el capstone no los define;
- que Exportación y Revisión quedaron fuera de este corte, si las dejaste fuera.
