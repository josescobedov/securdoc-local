# SecurDoc Local 📄🛡️

Herramienta web diseñada para proteger documentos sensibles (como DNI, NIE, pasaportes, facturas o contratos) antes de compartirlos por medios digitales. Aplica conversión a blanco y negro con ajuste de contraste y marcas de agua de seguridad diagonales, ejecutándose íntegramente en el navegador sin transferir archivos a ningún servidor externo.

---

## 🔒 Privacidad y Seguridad

- **Ejecución 100% en cliente:** Toda la manipulación de imágenes y páginas PDF ocurre en la memoria del navegador (usando Canvas API y WebAssembly/JS).
- **Sin envíos a servidores:** No existen peticiones backend ni almacenamiento externo. Puedes desconectar internet y la herramienta seguirá funcionando.
- **Prevención de suplantación:** Convierte copias en color a blanco y negro contrastado y sobreimprime marcas de agua diagonales difíciles de borrar sin degradar el texto del documento.

---

## 🚀 Características Principales

1. **Formatos soportados:**
   - Documentos PDF multipágina.
   - Imágenes en formato JPG, PNG y WebP.

2. **Capa Blanco y Negro:**
   - Algoritmo de luminancia perceptual (Rec. 709).
   - Control de contraste ajustable para garantizar legibilidad de sellos y textos pequeños.

3. **Marca de Agua Diagonal:**
   - Modo única diagonal con ajuste automático al largo de la página.
   - Modo mosaico repetido con rotación angular.
   - Delineado bicolor (halo claro y relleno oscuro) para visibilidad en fondos claros y oscuros.
   - Reparto en dos líneas para textos largos.

4. **Exportación:**
   - Generación directa de un nuevo PDF compuesto mediante jsPDF en alta resolución.

---

## 💻 Cómo utilizar el proyecto

### Uso local inmediato
No requiere instalación de Node.js, compilación ni dependencias previas:
1. Clona este repositorio o descarga los archivos.
2. Abre `index.html` en cualquier navegador web moderno (Chrome, Firefox, Safari, Edge).

### Publicación en GitHub Pages
Para utilizarlo desde cualquier dispositivo o móvil:
1. En tu repositorio de GitHub, ve a **Settings** > **Pages**.
2. En **Build and deployment**, selecciona **Source: Deploy from a branch**.
3. Elige la rama `main` y la carpeta `/(root)`.
4. Haz clic en **Save** y en un minuto tendrás tu enlace público listo.

---

## 🛠️ Tecnologías empleadas

- **HTML5 & Vanilla JavaScript**: Lógica de eventos y procesamiento de Canvas en memoria.
- **Tailwind CSS**: Estructura visual y componentes de interfaz.
- **PDF.js**: Extracción y rasterizado local de páginas PDF.
- **jsPDF**: Generación y exportación del archivo PDF final.

---

## 📄 Licencia

Este proyecto se distribuye bajo términos de código abierto para uso personal y profesional libre.
