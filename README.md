# GP2
ASSAF

## Cómo Compartir Documentos para Análisis

Este repositorio acepta documentos para análisis. Sigue estas instrucciones para compartir tus documentos de manera efectiva.

### Formatos Recomendados

Los formatos preferidos son:
- **PDF** - Formato universal, compatible con todos los sistemas
- **Markdown (.md)** - Ideal para documentos de texto con formato simple

También se aceptan documentos Word (.docx), pero se recomienda convertirlos a PDF o Markdown cuando sea posible.

### Métodos para Compartir Documentos

Hay tres formas principales de compartir documentos:

1. **Adjuntar en Issues de GitHub**
   - Ve a la pestaña "Issues" del repositorio
   - Crea un nuevo issue o comenta en uno existente
   - Arrastra y suelta tu archivo directamente en el cuadro de comentarios
   - GitHub aceptará archivos PDF, DOCX, imágenes y más

2. **Adjuntar en Conversaciones/Chat**
   - Si estás usando GitHub Discussions o cualquier chat relacionado
   - Simplemente arrastra y suelta o usa el botón de adjuntar archivos
   - Comparte el enlace generado

3. **Subir al Repositorio (Commit)**
   - Clona el repositorio: `git clone https://github.com/Alex-uni1/GP2.git`
   - Añade tu documento: `git add tu-documento.pdf`
   - Haz commit: `git commit -m "Añadir documento para análisis"`
   - Sube los cambios: `git push`
   - Luego, referencia el archivo en un issue con su ruta en el repositorio

### Conversión de DOCX a PDF o Markdown

Si tienes un documento Word (.docx) y deseas convertirlo a PDF o Markdown, aquí hay algunas opciones:

#### Convertir DOCX a PDF usando LibreOffice (Línea de Comandos)

LibreOffice ofrece una herramienta de línea de comandos muy útil:

```bash
# Instalar LibreOffice (si no lo tienes)
# En Ubuntu/Debian:
sudo apt-get install libreoffice

# En macOS con Homebrew:
brew install --cask libreoffice

# Convertir DOCX a PDF
libreoffice --headless --convert-to pdf "tu-documento.docx"

# O especificando el directorio de salida
libreoffice --headless --convert-to pdf "tu-documento.docx" --outdir ./output
```

#### Convertir DOCX a Markdown usando Pandoc

Pandoc es una herramienta excelente para convertir entre formatos:

```bash
# Instalar Pandoc
# En Ubuntu/Debian:
sudo apt-get install pandoc

# En macOS con Homebrew:
brew install pandoc

# Convertir DOCX a Markdown
pandoc "tu-documento.docx" -o "tu-documento.md"

# Con opciones adicionales para mejor formato
pandoc "tu-documento.docx" -o "tu-documento.md" --extract-media=./media
```

#### Otras Herramientas

- **Online**: Puedes usar convertidores en línea como [Zamzar](https://www.zamzar.com/) o [CloudConvert](https://cloudconvert.com/)
- **Microsoft Word**: Guardar como → PDF (disponible en Word mismo)
- **Google Docs**: Subir el DOCX → Archivo → Descargar → PDF o Markdown

### Documentos Existentes en el Repositorio

Los siguientes documentos ya están disponibles en el repositorio:

- [Actividad-S4_CO921 G_2026_VERANO (1).docx](./Actividad-S4_CO921%20G_2026_VERANO%20(1).docx) - Documento de actividad del curso CO921

### Consejos Adicionales

- **Nombres de Archivo**: Usa nombres descriptivos sin espacios (usa guiones o guiones bajos)
- **Tamaño**: GitHub tiene un límite de 25 MB para archivos individuales en issues
- **Privacidad**: Asegúrate de no compartir información sensible o personal
- **Descripción**: Siempre incluye una breve descripción de qué trata el documento

### Soporte

Si tienes problemas para compartir documentos o necesitas ayuda con las conversiones, abre un issue en el repositorio y el equipo te ayudará.
