# VHUMAN — Portal de Capacitaciones

Portal web estático para acceso a materiales de capacitación corporativa. Diseñado para ser publicado vía GitHub Pages y accedido por clientes directamente desde el navegador.

## Estructura

```
├── index.html                          # Portal principal — listado de programas
├── liderazgo.html                      # Programa de Liderazgo y Gerenciamiento
├── assets/
│   ├── style.css                       # Design system compartido
│   └── logo.svg                        # Logo VHUMAN vectorial
└── PROGRAMA DE FORTALECIMIENTO .../   # Materiales (PDFs, Excel, PPTX)
```

## Programas disponibles

### Programa de Fortalecimiento de Liderazgo y Gerenciamiento

| Módulo | Tema | Materiales |
|--------|------|-----------|
| 1 | Liderazgo Sistémico | Video (Drive) |
| 2 | Inteligencia Emocional | Video (Drive) |
| 3 | Comunicación Estratégica | Video (Drive) · 3 PDFs · Infografía |
| 4 | Gestión de Equipos de Alto Rendimiento | Video (Drive) · PDF · Infografía |
| 5 | Negociación y Resolución de Conflictos | Presentación PPTX |
| 6 | Gestión de Proyectos | PDF · 2 Excel (Cursograma · Gantt) |
| 7 | Finanzas para la Gestión | PDF |
| 8 | Gestión del Cambio y Transformación | PDF |

## Publicación (GitHub Pages)

1. Ir a **Settings → Pages** en el repositorio
2. Branch: `master` · Folder: `/ (root)`
3. Guardar — la URL queda en:

```
https://agallardo2802.github.io/ggs_capacitaciones_rrhh/
```

## Agregar un nuevo programa de capacitación

1. Crear una carpeta con los materiales en la raíz del repo
2. Duplicar `liderazgo.html` y renombrarlo (ej. `ventas.html`)
3. Actualizar el contenido de módulos y materiales en el nuevo HTML
4. Agregar una card en `index.html` apuntando al nuevo archivo

## Agregar materiales a un módulo existente

- **PDFs / Excel / PPTX**: copiá el archivo a la carpeta del programa y agregá un chip en el HTML correspondiente
- **Videos**: subí el video a Google Drive, compartilo con "Cualquier persona con el enlace" y actualizá el `href` del chip

## Videos en Google Drive

Los videos se sirven desde Google Drive para mantener el repositorio liviano. Para actualizar un link:

```html
<!-- Formato del chip de video -->
<a href="https://drive.google.com/file/d/FILE_ID/view?usp=drive_link"
   class="chip chip-video" target="_blank" rel="noopener">
  Clase grabada
</a>
```

Reemplazá `FILE_ID` con el ID del archivo en Drive (visible en la URL al abrir el archivo).

---

**VHUMAN Gestión de Talento** · Todos los derechos reservados
