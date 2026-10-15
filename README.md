# Póster Multipágina Pro 🖨️✨
> **Estudio Web de Preimpresión, División de Imágenes y Plano de Montaje para Pósteres Gigantes.**

[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-brightgreen?style=flat-square&logo=github)](https://9noir.github.io/multipage-poster-pro/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![Zero Backend](https://img.shields.io/badge/Privacy-100%25%20Client--Side-success?style=flat-square)](https://9noir.github.io/multipage-poster-pro/)
[![jsPDF Engine](https://img.shields.io/badge/PDF%20Engine-jsPDF%20v2.5-orange?style=flat-square)](https://github.com/parallax/jsPDF)

---

## 🌐 Demo en Vivo
Puedes utilizar la aplicación directamente desde tu navegador sin instalar nada:
👉 **[https://9noir.github.io/multipage-poster-pro/](https://9noir.github.io/multipage-poster-pro/)**

---

## 📌 ¿Qué es Póster Multipágina Pro?

**Póster Multipágina Pro** (`multipage-poster-pro`) es una aplicación web moderna y ligera pensada para diseñar, dividir y preparar cualquier fotografía, póster, plano arquitectónico, ilustración o gráfico de gran tamaño para ser impreso en impresoras estándar (de oficina o domésticas) en múltiples hojas (A4, A3, Carta, Oficio, etc.).

A diferencia de los divisores tradicionales o alternativas clásicas como *The Rasterbator*, esta herramienta incorpora un flujo completo de **estudio de preimpresión**:
- **Solapas de pegado superpuestas** milimétricas configurables.
- **Sistema de empalmes con coordenadas A-A** (`A1 ↔ A2`, `A1 ↕ B1`).
- **Miras de registro micrométricas** (⊕) para alinear las hojas con precisión milimétrica.
- **Plano maestro de armado** esquemático descargable e integrado al PDF final.
- **Exportación en alta resolución nativa** (hasta 400 DPI) con [jsPDF](https://github.com/parallax/jsPDF).

---

## 🚀 Características Principales

### 1. 🖼️ Carga y Transformación de Imagen
- **Arrastrar y reencuadrar**: Mueve la imagen libremente con el mouse o touchpad dentro del canvas.
- **Zoom continuo**: Desde 20% hasta 400% con rueda de ratón o slider.
- **Modos automáticos**:
  - *Cover* (Cubrir todo el póster manteniendo proporción).
  - *Contain* (Ajustar imagen completa sin recortar bordes).
  - *Stretch* (Estirar al 100% del área).
- **Herramientas de orientación**: Rotación en pasos de 90° y volteo de espejo horizontal y vertical.
- **Fondo configurable**: Selector de color para los márgenes vacíos y botón de recentrado rápido.

### 2. 📐 Formatos y Calculadora de Medidas
- Soporta formatos universales: **A4**, **A3**, **Carta (Letter)**, **Oficio (Legal)**, **Tabloide (Tabloid)** y dimensiones milimétricas **Personalizadas**.
- Orientación de hoja **Vertical (Portrait)** u **Horizontal (Landscape)**.
- Cuadrícula de hasta **20 columnas × 20 filas**.
- **Calculadora por Medida Deseada**: Introduce el ancho o alto deseado en centímetros (por ejemplo: `120 cm` de ancho) y la herramienta calculará automáticamente la cantidad óptima de hojas respetando la proporción de tu imagen.
- **Telemetría en tiempo real**: Muestra las medidas finales del póster armado (en cm) y el cálculo de **DPI efectivos de impresión** con avisos de calidad (Óptimo, Cartel o Baja resolución).

### 3. 🧩 Sistema de Preimpresión y Empalmes A-A
- **Solapa de Pegado Regulable**: Ajusta la superposición entre hojas contiguas (por ejemplo 12 mm o 15 mm).
- **Márgenes de Impresora**: Define los márgenes de hardware sin impresión (con presets rápidos: 0 mm sin borde, 5 mm estándar y 10 mm seguro).
- **Códigos de Empalme en Bordes**: Cada hoja imprime indicadores perimetrales claros para saber exactamente con qué hoja vecina ensamblar (`A1 ↔ A2` a la derecha, `A1 ↕ B1` abajo).
- **Miras de Registro Micrométricas (⊕)**: Cruces de alineación impresas al 20%, 50% y 80% de cada solapa.
- **Reserva de Pegamento (*Glue Strip*)**: Franja limpia de 5 mm sin tinta dentro de la solapa oculta para asegurar que el pegamento adhiera papel con papel sin degradarse por el toner o la tinta.
- **Modo Limpio Garantizado (*Clean Mode*)**: Los textos técnicos y marcas solo se imprimen en áreas que se recortan o en solapas que quedarán cubiertas por la hoja contigua; el frente visible del póster queda 100% impecable.

### 4. 🗺️ Plano Maestro de Armado (Assembly Blueprint)
- Genera automáticamente una hoja resumen con el diagrama numerado de la cuadrícula, medidas finales y la secuencia paso a paso de corte y ensamble.
- Puedes incluirla al **final del PDF**, al **principio (pág. 1)** o exportarla como imagen **PNG independiente**.

### 5. 🖨️ Exportación y Salida
- **PDF Completo para Imprimir**: Empaqueta todas las hojas ordenadas en un único archivo PDF listo para enviar a la impresora.
- **Selector de Calidad**:
  - *Rápida* (~190 DPI)
  - *Imprenta Pro* (~300 DPI)
  - *Ultra HD* (~400 DPI)
- **Impresión Directa del Navegador (`Ctrl + P`)**: Formateado con reglas CSS `@page` milimétricas nativas.

---

## 🔒 Privacidad y Rendimiento (100% Client-Side)

Toda la manipulación de imágenes, el recorte matricial y la compilación del archivo PDF se realizan **exclusivamente en tu navegador web** mediante la API Canvas de HTML5 y JavaScript.
- ❌ **Ninguna imagen es enviada a servidores externos**.
- 📶 **Funciona sin conexión a internet** (puedes guardar el archivo HTML y abrirlo offline).
- ⚡ Procesamiento rápido y sin límite de uso ni marcas de agua impuestas.

---

## 🛠️ Estructura del Proyecto

```text
multipage-poster-pro/
├── index.html       # Aplicación web completa y autónoma (HTML + CSS + JS)
├── LICENSE          # Licencia de código abierto MIT
└── README.md        # Documentación oficial del proyecto
```

---

## 💻 Ejecución Local

Si deseas correrlo localmente en tu computadora:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/9Noir/multipage-poster-pro.git
   cd multipage-poster-pro
   ```
2. Abre el archivo `index.html` en cualquier navegador web moderno (Chrome, Edge, Firefox, Brave, Safari):
   ```bash
   # En Windows PowerShell
   Start-Process index.html
   ```
   *No requiere Node.js, Python ni servidores backend.*

---

## 📄 Licencia

Este proyecto está bajo la licencia [MIT](LICENSE). Eres libre de usarlo, modificarlo y compartirlo para proyectos personales o comerciales.
