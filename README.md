# 🇯🇵 Nipones al Abordaje 2026 — App de viaje

Web-app de viaje (`index.html`) que se abre desde una **URL** y se puede **instalar como app** en
**iPhone y Android** (pantalla completa, con icono propio). Es una **PWA**: lleva un *web app manifest*
e iconos para que tanto Safari como Chrome la añadan a la pantalla de inicio.

> Esta versión es **pública y anónima** (para compartir con el grupo). Necesita **conexión** para
> abrirse (está hospedada en una URL); las fotos y los datos van dentro de la propia app.

---

## 📲 Cómo instalarla (iPhone y Android)

Abre la **URL** de la app en el navegador y añádela a la pantalla de inicio:

**iPhone (Safari):**
1. Abre la URL en **Safari**.
2. Toca **Compartir** (cuadro con flecha ↑) → **Añadir a pantalla de inicio**.
3. Aparece el icono **"Japón 2026"**; se abre a pantalla completa, como una app.

**Android (Chrome):**
1. Abre la URL en **Chrome**.
2. Menú **⋮** → **Instalar aplicación** (o **Añadir a pantalla de inicio**).
3. Aparece el icono **"Japón 2026"**; se abre a pantalla completa, como una app.

> 💡 También funciona simplemente abriéndola en cualquier navegador (móvil o PC), sin instalar.

---

## 🧭 Qué incluye

- **Inicio** — saludo, tarjeta de "Hoy" (o cuenta atrás antes del viaje) con foto, plan de mañana y accesos rápidos.
- **Días** — las 17 jornadas (viaje de ida + 15 días + regreso), cada una con **foto** y estado *Hoy / Hecho / Próximo*.
- **Día** — cabecera con foto, horarios bloque a bloque con una **curiosidad 💡 en cada visita**, hotel/barco de la noche, **"¿Sabías que…?"** y **"Para probar"** (gastronomía), botón *Abrir en Maps* y marcar como completado.
- **Viaje** — vuelos Qatar (horarios de ida y vuelta y enlaces al aeropuerto en Maps).
- **Hoteles** — fichas con *Maps / Llamar / Email / Web*.
- **¥/€** — conversor de moneda con tipo de cambio editable (botón propio en la barra inferior).
- **Lugares** — ~38 fichas **con foto**, descripción, consejo y dato curioso; filtros por ciudad y favoritos ⭐.
- **Mapa** — directorio de hoteles, templos, puertos… con *Abrir en Maps*.
- **Frases** — japonés + pronunciación con botón de **audio** 🔊 (voz del propio móvil).
- **SOS** — teléfonos de emergencia (seguro, Embajada de España en Tokio, 110/119 de Japón) con llamada directa y "qué hacer si…".
- **Checklist antes del viaje** — lista de equipaje marcable (se guarda lo marcado).

El **botón 🆘 rojo** está siempre visible en pantalla.

### 📷 Fotos reales
Las fotos de cada ciudad y lugar van **dentro de la app** (no se cargan de fuera), proceden de
**Wikimedia Commons / Wikipedia** (licencias libres) y están comprimidas. La app **arranca antes de
pintar las fotos**: el contenido funciona enseguida y las imágenes aparecen un instante después.

---

## 🚀 Despliegue (hosting)

Sube/sirve **toda la carpeta** (no solo el HTML) para que la instalación con icono funcione:

```
index.html              ← la app
manifest.webmanifest    ← define nombre, icono y modo "app" (Android)
apple-touch-icon.png    ← icono para iOS (180×180)
icon-192.png            ← icono PWA (Android)
icon-512.png            ← icono PWA (Android)
```

- **GitHub Pages:** Settings → Pages → *Deploy from a branch* → `main` → `/ (root)`.
  El repo debe ser **público** (Pages gratis solo en repos públicos). URL: `https://<usuario>.github.io/<repo>/`.
- **Cualquier host estático / túnel:** sirve la carpeta entera. Si solo sirves `index.html`,
  la app abre igual, pero Android no podrá instalarla con icono (le falta el manifest/iconos).

---

## ✏️ Cómo editar los datos

Abre `index.html` con un editor de texto y busca **`DATA`** (al principio del bloque `<script>`).
Los datos están en objetos fáciles de tocar: `TRIP`, `DAYS`, `FLIGHTS`, `HOTELS`, `PLACES`,
`PHRASES`, `EMERGENCY`, `CHECKLIST`. Cambia textos, horas o teléfonos sin tocar el diseño.

---

## 🔒 Notas

- Los **enlaces de Maps** abren la app de mapas (necesitan conexión).
- El **audio** de las frases usa la voz japonesa del móvil (si no está instalada, muestra solo la pronunciación).
- Tus marcas (días hechos, checklist, favoritos, tipo de cambio) se guardan **en tu dispositivo** (no se comparten).
- Versión pública **anonimizada**: no incluye datos personales (localizadores, teléfonos privados, direcciones).

¡Buen viaje! よい旅を (yoi tabi o) 🎌
