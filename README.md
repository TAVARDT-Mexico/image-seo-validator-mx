<p align="center">
  <a href="https://ag.tavardt.com/mx/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="1024" />
  </a>
</p>

# Analizador de SEO para Imagenes y Accesibilidad Web

[![Analizador SEO Imagenes](https://img.shields.io/badge/TAVARDT-Image%20SEO-5b3cf5.svg)](https://tools.tavardt.com/mx/analizador-seo-imagenes/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de integridad de texto alternativo, adopcion de formatos WebP y AVIF, dimensiones de estabilidad visual y metadatos sociales.

***

## Vectores de Riesgo e Impacto Operativo en la Entrega de Imagenes

La ausencia de texto alternativo genera barreras de accesibilidad e impide la indexacion visual en motores de busqueda en Mexico. Los textos genericos o nombres de camara restan relevancia semantica y limitan la visibilidad en busquedas organicas.

Distribuir imagenes pesadas en formatos antiguos agota los datos y alarga el tiempo de respuesta en conexiones moviles. La falta de dimensiones explicitas causa desplazamientos abruptos de pantalla y castiga las calificaciones de estabilidad visual.

***

## Capacidades Centrales de Auditoria Tecnica

* **Auditoria Critica de Texto Alternativo (Alt)**: Inspecciona cada etiqueta de imagen detectando la falta de alt, aplicando deducciones de hasta 35 puntos con alerta critica.
* **Filtrado de Descripciones Genericas**: Detecta terminos vagos como imagen o foto y nombres automaticos de archivo, deduciendo 5 puntos por caso hasta 15 puntos.
* **Adopcion de Formatos de Proxima Generacion**: Comprueba la presencia de WebP, AVIF y SVG frente a formatos heredados JPEG y PNG, con penalizaciones de hasta 20 puntos.
* **Control de Estabilidad de Layout (CLS)**: Verifica la presencia de atributos explicitos width y height, deduciendo 3 puntos por imagen sin dimensiones hasta 20 puntos.
* **Comprobacion de Carga Diferida (Lazy Loading)**: Analiza el uso del atributo loading='lazy' para asegurar la descarga asincrona de recursos fuera de pantalla.
* **Validacion de Metadatos Open Graph**: Confirma la declaracion de la etiqueta og:image para generar vistas previas atractivas, aplicando 10 puntos de penalizacion si falta.
* **Indice de Calidad de SEO Visual**: Calcula una calificacion de 0 a 100 categorizando los recursos en COMPLIANT, WARNING o CRITICAL.

***

## Instalacion y Ejecucion

Requiere Python 3.8 o superior utilizando unicamente bibliotecas estandar.

```bash
git clone https://github.com/TAVARDT-Mexico/image-seo-validator-mx.git
cd image-seo-validator-mx
python image_seo_scanner.py https://empresa.mx
```

Para generar la salida en formato estructurado JSON en procesos automatizados de auditoria:

```bash
python image_seo_scanner.py https://empresa.mx -j
```

***

## Preguntas Frecuentes (FAQ Tecnico)

### 1. Como afecta la ausencia de atributos alt a la indexacion visual y la accesibilidad?
Los motores de busqueda utilizan el texto alternativo para comprender el significado de las imagenes e indexarlas correctamente. La omision del atributo alt infringe los estandares de accesibilidad y bloquea la extraccion de datos por modelos de inteligencia artificial.

### 2. Por que el auditor penaliza descripciones genericas o nombres de archivo por defecto?
Terminos como imagen o codigos generados por camaras no aportan informacion semantica para personas con discapacidad visual. Los algoritmos de clasificacion consideran estas etiquetas como relleno superfluo y descartan su valor de posicionamiento.

### 3. Como ayuda la definicion explicita de dimensiones a mitigar el Cumulative Layout Shift?
Declarar los valores de width y height permite que el navegador calcule la proporcion y reserve el espacio necesario antes de descargar la imagen. Omitir estos parametros provoca desplazamientos repentinos del contenido y perjudica las metricas de Core Web Vitals.

### 4. Que ventajas tecnicas ofrecen los formatos WebP y AVIF sobre los archivos JPEG y PNG tradicionales?
Los formatos modernos proporcionan algoritmos de compresion avanzados que reducen el peso de las imagenes entre un veinticinco y un cincuenta por ciento sin perdida apreciable. Esta optimizacion acelera el tiempo de renderizado y reduce el consumo de datos moviles.

### 5. Por que es indispensable configurar la imagen Open Graph en la arquitectura web?
Las plataformas de mensajeria y los motores de respuesta leen los metadatos og:image para construir tarjetas visuales enriquecidas. La ausencia de esta etiqueta genera enlaces sin atractivo visual que sufren una disminucion considerable en la tasa de clics.

***

## Asesoria en Accesibilidad Visual y Optimizacion de Medios

Para portales de alto volumen y cumplimiento estricto de las directrices W3C WCAG, consulte con los ingenieros de **TAVARDT**.

***

## Enlaces Utiles

* **Portal Corporativo:** https://ag.tavardt.com/mx/
* **Suite de Diagnosticos:** https://tools.tavardt.com/mx/
* **Contacto Tecnico:** https://ag.tavardt.com/mx/contacto/

***

### Licencia
Distribuido bajo la Licencia MIT. Consulte el archivo LICENSE para mas detalles.

***

© 2026 TAVARDT. Todos los derechos reservados.
