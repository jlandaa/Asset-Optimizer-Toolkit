# Asset-Optimizer-Toolkit 🚀
![Status: Maintained](https://img.shields.io/badge/Status-Maintained-brightgreen?style=for-the-badge)
![License: MIT](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pillow](https://img.shields.io/badge/Pillow-013243?style=for-the-badge&logo=python&logoColor=white)
![Lighthouse](https://img.shields.io/badge/Google_Lighthouse-F44B21?style=for-the-badge&logo=google-lighthouse&logoColor=white)

Colección de scripts en **Python** diseñados para la automatización, procesamiento y optimización técnica de activos visuales destinados a sitios web y dashboards de alto rendimiento.

El objetivo principal es garantizar que las imágenes cumplan con los estándares de **Google Lighthouse**, equilibrando una carga ultra-rápida sin sacrificar la nitidez en pantallas de alta densidad (Retina).

## 🛠️ Funcionalidades Principales

* **Conversión a WebP con Analíticas:** Transformación de archivos PNG a WebP utilizando compresión *lossless* y reportando el ahorro exacto en MB y porcentaje.
* **Tratamiento de Transparencias:** Algoritmo de detección de fondos blancos (píxeles con RGB > 240) para su conversión automática a canales alfa transparentes.
* **Optimización (Lighthouse Ready):** Ajuste de dimensiones basado en el ancho de renderizado real del DOM (DPR 1.2x y 2x) para maximizar el rendimiento.
* **Generación de Favicons:** Creación automatizada de `apple-touch-icon` (180x180) y favicons estándar (32x32, 16x16) a partir de un archivo `.ico`.
* **Compresión de Perfil:** Script dedicado para fotos personales, reduciendo drásticamente el peso de archivos originales de alta resolución a formatos web eficientes.

---

## 📋 Estructura de los Scripts

| Archivo | Función |
| :--- | :--- |
| `procesar_logos.py` | Remoción de fondos blancos y conversión a PNG transparente. |
| `convert_to_webp_analytics.py` | Conversión masiva a WebP con reporte detallado de ahorro de espacio. |
| `generate_icons.py` | Generación de activos para navegadores y dispositivos iOS a partir de un `.ico`. |
| `optimizar_perfil.py` | Redimensionamiento (400x400) y compresión de fotos personales. |
| `optimizar_logos.py` | Optimización masiva de logos con anchos objetivos predefinidos. |
| `optimizar_logos_2.py` | Optimización (Display Width * 1.2) para nitidez en pantallas modernas. |
| `optimizar_logos_3.py` | Ajuste final basado en dimensiones exactas extraídas de reportes de Lighthouse. |

---

## 🚀 Instalación y Uso

### 1. Requisitos
Requiere Python 3.x y la biblioteca **Pillow**

```bash
pip install Pillow
```

### 2. Configuración de Rutas: 
Edita las variables de directorio de entrada y salida en el script que desees ejecutar (se recomienda utilizar rutas relativas)
```python
# Ejemplo de configuración de rutas
ORIGEN = "./Logos"
DESTINO = "./Logos_Optimized"
```
### 3. Ejecución: 
Ejecuta el script deseado desde la terminal
```bash
# Ejemplo: optimización basada en métricas de Lighthouse
python optimizar_logos_3.py
```

## 💻 Tecnologías Utilizadas
* **Lenguaje:** Python 3.x
* **Procesamiento de Imagen:** Pillow (PIL)
* **Formatos Soportados:** WEBP, PNG, JPG, ICO.

---
👨‍💻 **Juan Manuel Landa** — *Computer Engineer | Data Analyst & BI Consultant*  
🔗 [LinkedIn](https://ar.linkedin.com/in/juan-manuel-landa/en) • 🌐 [Portfolio](https://juan-manuel-landa.netlify.app/) • ✉️ [Contacto](mailto:jmlanda93@gmail.com)
