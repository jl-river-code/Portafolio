================================================================================
          UNIVERSIDAD DEL VALLE DE GUATEMALA - FACULTAD DE INGENIERÍA
                   DEPARTAMENTO DE CIENCIAS DE LA COMPUTACIÓN
                       CC3091 – INGENIERÍA DE SOFTWARE 2
                               SEMESTRE II – 2026
================================================================================
           PORTAFOLIO FINAL DE PROYECTO: INVERSIONES ELOHIM SOLUTION
                   (DM HUB - MULTI-TENANT E-COMMERCE PLATFORM)
================================================================================

EQUIPO DE DESARROLLO (GRUPO NO. 5):
- Angel Chavez          – Carné: 24248
- Iván Morataya         – Carné: 16667
- Arturo Lima           – Carné: 24683
- José Rivera           – Carné: 24376
- Giancarlo Sagastume   – Carné: 24278
- René Abella           – Carné: 24290

Catedrático: Pablo Andrés Barreno Koch

--------------------------------------------------------------------------------
1. DESCRIPCIÓN GENERAL DEL PORTAFOLIO
--------------------------------------------------------------------------------
Este portafolio recopila y estructura formalmente toda la evidencia, artefactos,
código fuente, infraestructura y tareas de mejora de procesos desarrollados a lo
largo de los dos semestres de formación profesional:
  - Fase 1: Ingeniería de Software 1 (Semestre I) - Análisis, Diseño y Sprints 1 a 4.
  - Fase 2: Ingeniería de Software 2 (Semestre II) - Sprints 5 a 10, Testing,
            Mantenimiento, Evaluaciones UX, RTF e Infraestructura Productiva.

El sistema desarrollado, "Inversiones Elohim Solution (DM Hub)", es una plataforma
de comercio electrónico multi-tienda (multi-tenant) de alto rendimiento, diseñada
con arquitectura limpia, soporte transaccional ACID, catálogo de productos, pasarela
de pagos Stripe e infraestructura en contenedores Docker orquestada en Dokploy.

--------------------------------------------------------------------------------
2. ESTRUCTURA Y DISTRIBUCIÓN DE CARPETAS
--------------------------------------------------------------------------------
La estructura del portafolio se organiza en estricto cumplimiento con la "Guía de
entrega Final del Proyecto" emitida por el Departamento de Ciencias de la
Computación de la UVG:

Portafolio/
│
├── README.txt                               <- Este archivo de descripción general
│
├── Análisis_y_Diseño/                        <- Etapas de análisis, diseño y empatía
│   ├── README.txt                           <- Guía completa de análisis, diseño y anexos
│   └── Documentos/                          <- Documentos de entrega y User Story Map
│       ├── Documentos.txt
│       ├── Corte 1 Comprendiendo el Problema.pdf
│       ├── Corte 2 Captura de Requisitos.pdf
│       ├── Corte 3 Analisis y Diseño.pdf
│       ├── User_Story_Map.pdf
│       └── Anexos/                          <- Materiales de apoyo, prototipos y BD
│           ├── Anexos.txt
│           ├── Prototipos Lean UX-1.pdf
│           └── Proyecto no.1 Integracion Ing. Software (3).pdf
│
├── Implementación/                          <- Organización de los 10 Sprints Scrum
│   ├── README.txt                           <- Guía completa de Sprints 1-10 y mejoras
│   ├── Implementacion.txt
│   ├── Sprint 1/                            <- Inicio del programa (Ing. Soft 1)
│   ├── Sprint 2/                            <- Vista cliente (Ing. Soft 1)
│   ├── Sprint 3/                            <- Prototipo interactivo cliente
│   ├── Sprint 4/                            <- Vista administrativa backoffice
│   ├── Sprint 5/                            <- Rediseño, RTF 1 y validación
│   │   ├── RTF_recibido/                    <- RTF recibida del Equipo 4
│   │   └── tarea_de_mejora_el_proceso/      <- Tarea de Mejora 1: RTF Vida Sana
│   ├── Sprint 6/                            <- Quality of Life Changes
│   ├── Sprint 7/                            <- Deuda técnica y Tarea de Mejora 2 (UX 1)
│   ├── Sprint 8/                            <- Mantenimiento y Tarea de Mejora 3 (UX 2)
│   ├── Sprint 9/                            <- CI/CD y Tarea de Mejora 4 (RTF 2 + OWASP)
│   └── Sprint 10/                           <- Cierre y Tarea de Mejora 5 (Lean)
│
├── Sistema desarrollado/                    <- Código, entorno Docker y repositorios
│   ├── CC3090-inversiones-elohim-solution.zip <- Código fuente y entorno contenerizado
│   ├── SW.txt                               <- Guía rápida de ejecución con Docker
│   └── Repositorio_Links.txt                <- Enlaces a repositorios GitHub y Jira
│
└── Tecnología_Usada/                        <- Decisiones y justificaciones técnicas
    ├── README.txt                           <- Descripción breve de cada archivo de la carpeta
    ├── 03_Seleccion_Persistencia_de_datos.pdf
    ├── Tarea investigativa II.pdf
    ├── Tarea 3 (2)-1.pdf
    ├── Tarea investigativa Docker.pdf
    └── Tecnologias_Usadas.txt               <- Resumen ejecutivo de arquitectura

--------------------------------------------------------------------------------
3. GUÍA DE NAVEGACIÓN Y RESUMEN DE CONTENIDO POR SECCIÓN
--------------------------------------------------------------------------------

[1] Análisis_y_Diseño/ (Consulte Análisis_y_Diseño/README.txt):
    Reúne los tres cortes académicos de la etapa de especificación inicial:
    - Corte 1: Proceso de Design Thinking, empatía y comprensión de la problemática.
    - Corte 2: Elicitación y especificación de Requisitos Funcionales y No Funcionales.
    - Corte 3: Modelado de dominio, diagramas de arquitectura, componentes y datos.
    - User Story Map: Mapeo visual y secuencial de todas las épicas, actividades y
      slicing de entregas por release.
    - Anexos: Wireframes y prototipos Lean UX, además del diseño relacional inicial.

[2] Implementación/ (Consulte Implementación/README.txt):
    Contiene diez carpetas independientes (Sprint 1 a Sprint 10). En el archivo
    `Implementación/README.txt` se desglosa el objetivo de cada iteración, el
    documento entregable formal y el detalle de las Tareas de Mejora al Proceso
    (Revisiones Técnicas Formales RTF, pruebas de experiencia de usuario UX en
    laboratorio, mitigación OWASP y principios Lean).

[3] Sistema desarrollado/ (Consulte Sistema desarrollado/SW.txt):
    Proporciona los entregables ejecutables del software:
    - Archivo .zip con el código fuente del monorepositorio y el entorno Docker listo.
    - Documento `SW.txt` con los pasos concisos de ejecución con Docker Compose.
    - Enlaces oficiales a GitHub y al tablero de seguimiento en Atlassian Jira.

[4] Tecnología_Usada/ (Consulte Tecnología_Usada/README.txt):
    Documenta los estudios y tareas de selección tecnológica: framework de
    desarrollo frontend (Next.js), motor de persistencia (PostgreSQL + EF Core),
    herramientas de automatización y pruebas (xUnit/Moq), e infraestructura (Docker).

================================================================================
