# 🍼 Gestación Familiar - Control de Embarazo

Una aplicación web progresiva (PWA) diseñada para el seguimiento del embarazo, calculando la semana de gestación y proporcionando datos curiosos de desarrollo y conversación semana a semana.

## 📱 Funcionalidades

* **Calculadora de Gestación:** Determina la semana actual y la Fecha Probable de Parto (FPP) en base a la Fecha de la Última Regla (FUR).
* **Gráfica de Crecimiento:** Un diagrama alimentado por `Chart.js` que muestra el desarrollo del feto a lo largo de las semanas.
* **Hitos Médicos:** Panel con enlaces rápidos a las pruebas principales (Eco 12 semanas, ecografía morfológica, etc.).
* **App PWA (Offline e Instalable):** Al entrar en navegadores móviles (Chrome o Safari) sugerirá la instalación en la pantalla de inicio para funcionar en modo offline gracias a su *Service Worker*.

## 🚀 Despliegue Local

Para que la PWA y su Service Worker puedan ser probados localmente, tienes que servir la carpeta mediante un servidor HTTP básico. Abre la terminal en esta carpeta y lanza:

```bash
npx http-server -p 8000
```

O si prefieres usar Python:

```bash
python -m http.server 8000
```

A continuación, dirígete a `http://localhost:8000` (o a tu IP de red local para probarlo en el teléfono).

## 🛠 Tecnologías empleadas

* HTML, Vanilla CSS (`index.html`) y Vanilla JavaScript.
* `Tailwind CSS` a través de CDN, para dar los estilos responsive.
* `Chart.js` vía CDN.
* Service Worker + JSON Manifest (`sw.js` y `manifest.json`).
