# ⚔️ Karioz Handbook Compiler (Compilador JSON a Web/Markdown)

Esta aplicación web autónoma permite arrastrar y soltar (drag & drop) cualquier archivo JSON exportado desde **Foundry VTT** (por ejemplo: `fvtt-JournalEntry-reglas-de-juego-*.json`, `cualidades`, `magia`, `clases`, etc.) para renderizarlo inmediatamente con la interfaz visual oficial de **Karioz Handbook** y exportarlo fácilmente.

---

## 🚀 Características principales

1. **Drag & Drop de Archivos JSON:**
   - Permite arrastrar un solo archivo JSON o múltiples archivos a la vez.
   - Procesa automáticamente capítulos y páginas manteniendo el orden correcto.

2. **Visualizador e Interfaz Interactiva:**
   - Formateo automático de cartas emergentes (Callout Cards) para habilidades y conjuros.
   - Tablas adaptativas y diseño responsive.
   - Navegación lateral con buscador en tiempo real de páginas y reglas.
   - Selector de tema (Estilo Fantasía Oscura / Estilo Pergamino Clásico).

3. **Compilación y Exportación:**
   - **Descargar Handbook HTML:** Genera un archivo `.html` compilado e independiente que se puede abrir en cualquier navegador o compartir.
   - **Exportar .MD:** Convierte el JSON/HTML directamente a formato Markdown estructurado (`.md`).
   - **Imprimir / Guardar como PDF:** Estilos CSS optimizados para exportar a PDF en alta calidad con un solo clic.

---

## 📂 Cómo compartirlo con tu amigo

Existen dos opciones sencillas para compartirlo:

### Opción 1: Directa (Sin instalación)
Solo envíale la carpeta `karioz_compiler` o directamente el archivo `index.html`. 
Cualquier persona puede abrir `index.html` haciendo **doble clic** en su navegador (Chrome, Edge, Firefox, Brave, etc.) sin necesidad de instalar Python, Node.js ni ningún servidor backend.

### Opción 2: Compilación a Ejecutable (.exe)
Si deseas convertir la interfaz en una aplicación de escritorio `.exe`:
- Puedes usar **NW.js** o **Electron**:
  ```bash
  npx nativefier --name "Karioz Compiler" "file:///ruta/a/karioz_compiler/index.html"
  ```
- O empaquetar el archivo `index.html` con herramientas ligeras como **Webview App** o **HTML to EXE Converters**.
