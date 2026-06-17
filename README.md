# 🇯🇵 Nipones al Abordaje 2026 — App de viaje

App de viaje **en un solo archivo** (`nipones-2026.html`). Funciona **100 % sin internet**:
todo (diseño, datos y lógica) va dentro del propio archivo. No necesita instalación, ni servidor, ni conexión.

---

## 📲 Cómo llevarla en el iPhone

1. **Pasa el archivo `nipones-2026.html` al iPhone** (por AirDrop, email, WhatsApp a ti mismo, o iCloud Drive).
2. Guárdalo en la app **Archivos** (en "iCloud Drive" o "En mi iPhone").
3. Ábrelo: toca el archivo → se abre en **Safari**. ¡Listo, ya funciona sin datos!

### (Opcional) Tenerla como una app con icono
Para lanzarla rápido desde la pantalla de inicio:
1. Ábrela en Safari.
2. Toca **Compartir** (cuadro con flecha ↑) → **Añadir a pantalla de inicio**.
3. Aparecerá un icono "Japón 2026" que abre la app a pantalla completa.

> 💡 Funciona igual en Android (abrir con Chrome) y en cualquier ordenador (doble clic).

---

## 🧭 Qué incluye

- **Inicio** — saludo, tarjeta de "Hoy" (o cuenta atrás antes del viaje) con **ilustración**, plan de mañana y accesos rápidos.
- **Días** — las 18 jornadas (previo + viaje de ida + 15 días + regreso), cada una con **imagen** y estado *Hoy / Hecho / Próximo*.
- **Día** — cabecera con foto, horarios bloque a bloque con una **curiosidad 💡 en cada visita**, traslados, hotel/barco de la noche, **"¿Sabías que…?"** y **"Para probar"** (gastronomía), botón *Abrir en Maps* y marcar como completado.
- **Viaje** — vuelos Qatar (horarios de ida y vuelta y enlaces al aeropuerto en Maps).
- **Hoteles** — fichas con *Maps / Llamar / Email / Web* y código de reserva.
- **¥/€** — conversor de moneda (ahora con **botón propio** en la barra inferior), con tipo de cambio editable.
- **Lugares** — ~38 fichas **con ilustración**, descripción, consejo y dato curioso; filtros por ciudad y favoritos ⭐.
- **Mapa** — directorio de hoteles, templos, puertos, estaciones… con *Abrir en Maps*.
- **Frases** — japonés + pronunciación con botón de **audio** 🔊 (voz del iPhone).
- **SOS** — teléfonos de emergencia (seguro, Jesús, embajada, 110/119) con llamada directa y "qué hacer si…".
- **Checklist antes del viaje** — lista de equipaje marcable (se guarda lo marcado).

El **botón 🆘 rojo** está siempre visible en pantalla.

### 📷 Fotos reales (incrustadas)
La app lleva **fotos reales** de cada ciudad y lugar **incrustadas dentro del propio archivo** (en base64), así que
**se ven sin conexión**. El archivo pesa ~1 MB (comprimido a propósito para que **abra bien en la vista previa de Archivos**).
Las imágenes proceden de **Wikimedia Commons / Wikipedia** (licencias libres). Además, la **app arranca antes de cargar las
fotos**: si el móvil tarda con las imágenes, el contenido ya funciona y las fotos aparecen un instante después.
Si alguna foto no te gusta, dime el lugar y la cambio.

---

## ✏️ Cómo editar o completar datos

Abre `nipones-2026.html` con cualquier editor de texto y busca **`DATA`** (cerca del inicio del bloque `<script>`).
Los datos están en objetos fáciles de tocar: `TRIP`, `DAYS`, `FLIGHTS`, `TRAINS`, `VANS`, `HOTELS`,
`PLACES`, `PHRASES`, `EMERGENCY`, `CHECKLIST`. Cambia textos, horas o teléfonos sin tocar el diseño.

### Pendiente de añadir (cuando lo tengas)
- **Certificado individual del seguro** (nº de certificado, nombres de asegurados y fechas de cobertura).
- Teléfono del **Hotel Villa Fontaine (Tokio)** si lo facilita el organizador.
- Localizadores de crucero/vuelos *(los gestiona el organizador; la app ya lo indica)*.

### Añadir un PDF para verlo sin internet
Como es un archivo offline, un PDF se puede **incrustar en base64** dentro del HTML (engorda el archivo;
solo recomendable para 1–2 documentos clave, p. ej. la póliza). Dímelo y lo integro.

---

## 🔒 Notas

- Los **enlaces de Maps** abren la app de mapas y necesitan conexión puntual; el resto funciona sin datos.
- El **audio** usa la voz japonesa del iPhone (Ajustes → Accesibilidad → Contenido leído → Voces, si no la oyes).
- Tus marcas (días hechos, checklist, favoritos, tipo de cambio) se guardan **en tu móvil** (no se comparten).

¡Buen viaje! よい旅を (yoi tabi o) 🎌
