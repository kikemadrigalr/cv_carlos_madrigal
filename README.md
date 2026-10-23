# CV — Carlos Enrique Madrigal Ramos

<p align="center">
  <strong>Desarrollador Backend .NET · APIs REST escalables · Testing & Full Stack Angular</strong><br>
  Venezuela / Colombia · <a href="mailto:carlosmad03@gmail.com">carlosmad03@gmail.com</a> · <a href="https://wa.me/573127580552">+57 312 758 0552</a> / +58 422 716 0862<br>
  <a href="https://linkedin.com/in/carlosmad03">LinkedIn</a> · <a href="https://github.com/kikemadrigalr">GitHub</a>
</p>

---

## Descripción

Código fuente de mi currículum profesional, gestionado con [RenderCV](https://rendercv.com/). El CV se define en un único archivo YAML (`cv-carlos-madrigal_CV.yaml`) y se compila a PDF, HTML, Markdown y PNG. El YAML es la fuente de verdad; este README es un resumen.

---

## Perfil Profesional

Desarrollador backend con **5 años de experiencia** diseñando y manteniendo APIs REST robustas y escalables con .NET. Enfoque API-first con OpenAPI/Swagger como contrato de integración entre frontend y backend, y foco en código de alta calidad, refactors seguros y code reviews. Complemento con desarrollo Full Stack en Angular sobre design systems reutilizables.

Trayectoria completa en el ecosistema .NET: desde **.NET Framework 4.5 con Web Forms** en sistemas de gestión interna hasta **.NET 6–10** en plataformas clínicas en producción. Pruebas automatizadas con **xUnit** y **Playwright**, dominio de **SQL Server**, e integración de **IA** (Claude Code, Cursor, MCP) en el ciclo de desarrollo. Experiencia remota (sector salud y farmacéutico) y presencial (otros sectores).

---

## Experiencia Profesional

| Empresa | Cargo | Período | Stack principal |
|---------|-------|---------|-----------------|
| **TBTB Global** | Desarrollador Full Stack | 2023 – Actualidad | .NET 6–10, Angular 16/18, SQL Server, xUnit, Playwright, Azure |
| **Empresas Andinas** | Analista de Sistemas – Desarrollo | 2018 – 2020 | .NET Framework 4.5, ASP.NET Web Forms (ASPX), SQL Server, SSRS, IIS |
| **Delegación de Deportes – UDO** | Prácticas Profesionales | 2016 | Análisis de sistemas |

---

## Educación

- **Licenciado en Informática** — Universidad de Oriente (UDO), Venezuela, 2019

---

## Proyectos Destacados

| Proyecto | Período | Descripción |
|----------|---------|-------------|
| **DxOne — Programa de Diagnóstico LATAM** | 2026 | Solución regional para el diagnóstico de enfermedades raras de una farmacéutica global en Colombia, México, Argentina y Chile, que engloba tres programas antes operados en plataformas independientes. Módulos de Médicos, Pacientes y Red Dx en DxOne Connect, sincronización con app móvil, flujo de solicitudes diagnósticas e hypercare. .NET 8, Angular, SQL Server, Azure, Clean Architecture. |
| **TBTB Connect 2.0** | 2025 – 2026 | CRM operativo para clientes farmacéuticos: actividades con médicos y pacientes, seguimiento de procesos clínicos y gestión de toma y transporte de muestras. Módulos genéricos construidos por configuración SQL. |
| **RDSTP** | 2025 – 2026 | Ecosistema modular para la trazabilidad de muestras médicas: registro de sample, TRF, tracking de muestras y paquetes hasta el laboratorio. Backend .NET. |
| **RDGENPP** | 2024 | Sistema de seguimiento de muestras de pacientes entre laboratorios y centros de salud. |
| **Galexito — Sistema de gestión interno** | 2018 – 2020 | Módulos web en .NET Framework 4.5 con Web Forms y SQL Server en IIS, reportes gerenciales con SSRS y automatización de cartas de trabajo en RRHH. |
| **My home OI** | 2018 – 2020 | Sitio web de organización inmobiliaria (HTML5, CSS3, Bootstrap, JavaScript, jQuery). |

---

## Habilidades Técnicas

**Backend** — C#, .NET 6–10, .NET Framework 4.5 (ASP.NET Web Forms / ASPX), ASP.NET MVC, REST API, Entity Framework, API-first con OpenAPI/Swagger, Python (fundamentos)

**Testing & Calidad** — xUnit (unitarias e integración), Playwright (E2E), code reviews, refactorización, principios SOLID

**Bases de Datos** — SQL Server (procedimientos almacenados, optimización, reporting), MySQL

**Frontend** — Angular 14/16/18 (componentes, módulos, servicios, lazy loading, design systems), JavaScript ES6+, HTML5, CSS3, Bootstrap

**Herramientas** — Git, Visual Studio, Postman

**Inteligencia Artificial** — Claude Code y Cursor (uso diario: generación, refactorización, debugging, documentación) · MCP (integración de IA con APIs internas; Playwright MCP para E2E dirigidas por IA) · Gemini CLI y ChatGPT (investigación y prototipado)

---

## Cursos

Claude AI · Claude Code · Fundamentos de Python · APIs con .NET · Entity Framework · Principios SOLID con C# y .NET · Fundamentos de C# con .NET · ASP.NET Core · POO · Git y GitHub · Fundamentos de JavaScript · Frontend Developer — Platzi
IA para Programadores — educacionIT · SQL Basic & Intermediate — HackerRank

---

## Idiomas

| Idioma | Nivel |
|--------|-------|
| Español | Nativo |
| Inglés | B1 |

---

## Datos de Interés

- Gran capacidad de aprendizaje autodidacta y adopción acelerada de nuevas tecnologías
- Experiencia en modalidades remota, presencial e híbrida, con adaptabilidad a distintos equipos y sectores
- Músico trompetista profesional

---

## Estructura del Proyecto

```
cv_carlos_madrigal/
├── cv-carlos-madrigal_CV.yaml   # Fuente del CV (RenderCV) — única fuente de verdad
├── README.md                    # Este resumen
├── CLAUDE.md                    # Contexto para Claude Code
├── .gitignore
└── rendercv_output/             # Generado (PDF, HTML, MD, PNG) — ignorado por Git
```

---

## Uso

Requisitos: Python 3.8+ y RenderCV (`pip install rendercv`).

```bash
# Todos los formatos → rendercv_output/
rendercv render cv-carlos-madrigal_CV.yaml

# Solo PDF
rendercv render cv-carlos-madrigal_CV.yaml --pdf-only
```

Salida: `rendercv_output/Carlos_Enrique_Madrigal_Ramos_CV.{pdf,html,md,png}`.

Antes de generar, actualizar `settings.current_date` en el YAML (o eliminar la línea para usar la fecha del sistema).

---

## Configuración

Tema **Classic** de RenderCV, idioma español, plantilla de educación personalizada para títulos largos, iconos FontAwesome (`phone`, etc.).

---

## Licencia

Uso personal. El contenido es propiedad de **Carlos Enrique Madrigal Ramos**.

<p align="center">
  <em>Última actualización: Octubre 2026</em>
</p>
