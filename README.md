# Zeus Tablero

Dashboard de Gestion de Proyectos y Transformacion Digital
Construido con Google Apps Script + Google Sheets

---

## Que es Zeus Tablero?

Zeus Tablero es una aplicacion web interna construida sobre Google Apps Script
que permite gestionar proyectos estrategicos, ejes de transformacion, personas
y permisos desde una interfaz moderna conectada a Google Sheets.

## Arquitectura

La aplicacion sigue una arquitectura frontend/backend dentro de Google Apps Script:

- Backend (.gs): Logica de negocio, autenticacion OAuth, gestion de datos en Sheets
- Frontend (.html): Interfaz de usuario servida via HtmlService

## Estructura del Proyecto

```
zeus-tablero/
├── Admin.gs              # Panel de administracion y parametrizacion
├── Auth.gs               # Autenticacion OAuth cross-domain manual
├── Config.gs             # Configuracion del sistema y constantes
├── Main.gs               # Punto de entrada (doGet) y utilidades
├── Permisos.gs           # Gestion de permisos y roles de usuario
├── Proyectos.gs          # Gestion de proyectos y ejes estrategicos
├── Sheets.gs             # Capa de acceso a Google Sheets
├── Social.gs             # Funciones sociales y de equipo
├── Estilos.html          # Estilos CSS del tablero
├── Index.html            # Pagina principal y estructura HTML
├── Cliente_Estado.html   # Gestion de estado del cliente
├── Cliente_Eventos.html  # Manejadores de eventos del cliente
├── Cliente_Init.html     # Inicializacion y configuracion del cliente
├── Cliente_Modales.html  # Modales y dialogos de la interfaz
├── Cliente_Paneles.html  # Paneles de la interfaz principal
└── Cliente_Vistas.html   # Vistas y renderizado de datos
```

## Funcionalidades

- Autenticacion OAuth sin libreria externa (cross-domain manual)
- Gestion de roles y permisos por usuario y seccion
- Dashboard de proyectos con ejes estrategicos, estados y responsables
- Panel de personas con gestion de equipos y jefaturas
- Modo prueba para administradores
- Interfaz responsive con modales, paneles y vistas dinamicas

## Tecnologias

| Tecnologia | Uso |
|---|---|
| Google Apps Script | Backend y hosting |
| Google Sheets | Base de datos |
| HTML/CSS/JS | Frontend |
| OAuth 2.0 | Autenticacion |

## Autor

Jose Miguel Ochoa
Director de Transformacion Digital -- Dra Skin
LinkedIn: https://www.linkedin.com/in/jose-miguel-o/

---

Proyecto interno de transformacion digital -- Dra Skin 2026
