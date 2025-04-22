# Guía para Agregar Archivos a la Estructura de Documentación

Este archivo `README.md` explica cómo agregar nuevos archivos dentro de la estructura predefinida de documentación técnica y proyectos. El objetivo es mantener todo organizado y de fácil acceso.

## Estructura Principal del Proyecto

El proyecto tiene una estructura de carpetas organizada para almacenar Playbooks, Scripts, Diagramas, Recursos, Clientes, Backups y Proyectos.

### Estructura General:

DocumentacionTecnica/
│
├── 📁 01_playbooks
│   ├── 📁 01_dns
│   │   └── 01_cloudflare_crear-registro-a_v1.0.md
│   ├── 📁 02_linux
│   │   └── 01_ubuntu_configuracion-firewall_v1.0.md
│   ├── 📁 03_windows
│   │   └── 01_ad_crear-usuarios_v1.2.md
│   ├── 📁 04_erp
│   │   └── 01_odoo17_instalacion_v1.0.md
│   └── 📁 05_firewall
│       ├── 📁 01_pfsense
│       │   └── 01_procedimientos-creacion.md
│       └── 📁 02_fortinet
│           └── 01_procedimientos-creacion.md
│
├── 📁 02_scripts
│   ├── 📁 01_bash
│   ├── 📁 02_python
│   └── 📁 03_powershell
│
├── 📁 03_diagramas
│   ├── 📁 01_red
│   ├── 📁 02_arquitectura
│   └── 📁 03_servicios
│
├── 📁 04_recursos
│   ├── 📁 01_comandos
│   ├── 📁 02_plantillas
│   └── 📁 03_guias-externas
│
├── 📁 05_clientes
│   ├── 📁 01_empresaX
│   └── 📁 02_empresaY
│
└── 📁 06_backups
    └── 📁 01_versiones-antiguas



## Cómo Agregar Nuevos Archivos

Para agregar nuevos archivos a la estructura, sigue los pasos descritos a continuación:

### 1. **Determina en qué categoría debe ir el archivo:**
   - **Playbooks:** Archivos de procedimientos detallados para la implementación o configuración de servicios.
   - **Scripts:** Archivos de código utilizados para automatización o scripts específicos en Bash, Python o PowerShell.
   - **Diagramas:** Archivos gráficos como diagramas de red, arquitectura o flujos de servicio.
   - **Recursos:** Plantillas, guías externas o comandos útiles.
   - **Clientes:** Información específica o documentación relacionada con proyectos de clientes.
   - **Backups:** Copias de seguridad de la documentación o proyectos antiguos.

### 2. **Crear la estructura de carpetas si es necesario:**
   Si la carpeta correspondiente no existe en la estructura, créala dentro de la carpeta principal donde debe ir el archivo.

### 3. **Nombrar el archivo:**
   Los archivos deben tener nombres descriptivos y seguir una convención de versiones, por ejemplo:
   - `01_configuracion-firewall_v1.0.md`
   - `02_procedimiento-implementacion_v2.0.md`

### 4. **Agregar contenido:**
   Agrega la documentación, scripts o diagramas necesarios al archivo en formato adecuado (por ejemplo, Markdown, scripts de código, imágenes, etc.).

### 5. **Realizar un commit:**
   Si estás utilizando un sistema de control de versiones como Git, realiza un commit para guardar los cambios y mantener un historial de versiones.

### 6. **Revisar y actualizar la documentación:**
   Si agregas o actualizas archivos que afectan a otras partes de la estructura, asegúrate de revisar y actualizar cualquier documentación relacionada.


Siguiendo estos pasos, podrás agregar archivos de manera organizada a la estructura de documentación y mantener todo bien organizado para su fácil acceso y mantenimiento.
