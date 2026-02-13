# Página de Banda de Metal - Guía de Personalización

## 🎸 Descripción

Página web oscura y atmosférica para banda de Metal con logo central clickeable que muestra múltiples enlaces.

## 📂 Archivo

**Ubicación:** `/var/www/datrevil/band.html`

## 🎨 Características

- ✅ Diseño completamente oscuro y negro
- ✅ Efecto de niebla/humo animado
- ✅ Partículas flotantes tipo brasas
- ✅ Viñeta para efecto cinematográfico
- ✅ Logo central con efecto de brillo rojo al pasar el mouse
- ✅ Menú emergente con enlaces múltiples
- ✅ Todos los enlaces se abren en nueva pestaña
- ✅ Animaciones suaves y atmosféricas
- ✅ Responsive (adaptable a móviles)

## 🔧 Personalización

### 1️⃣ Cambiar el nombre de la banda

**Busca la línea 107:**

```html
<h1 class="band-name">METAL</h1>
```

Cambia "METAL" por el nombre de tu banda.

### 2️⃣ Usar un logo (imagen) en lugar de texto

**Paso 1:** Sube tu logo a la carpeta `/var/www/datrevil/img/`

**Paso 2:** En la línea 105, descomenta y modifica:

```html
<!-- Descomenta esta línea y cambia el nombre del archivo -->
<img src="img/tu-logo.png" alt="Band Logo" class="band-logo">
```

**Paso 3:** Comenta o elimina la línea del texto:

```html
<!-- <h1 class="band-name">METAL</h1> -->
```

### 3️⃣ Agregar tus enlaces

**Busca la línea 123-140.** Ahí verás la sección de enlaces:

```html
<!-- AQUÍ AGREGAS TUS ENLACES -->
<a href="TU_LINK_AQUI" target="_blank" class="link-item">
    <span>🎵 NOMBRE DEL ENLACE</span>
</a>
```

**Ejemplo completo:**

```html
<a href="https://www.youtube.com/@tubanda" target="_blank" class="link-item">
    <span>🎵 YouTube</span>
</a>
<a href="https://open.spotify.com/artist/123456" target="_blank" class="link-item">
    <span>🎧 Spotify</span>
</a>
<a href="https://www.instagram.com/tubanda" target="_blank" class="link-item">
    <span>📷 Instagram</span>
</a>
<a href="https://tubanda.bandcamp.com" target="_blank" class="link-item">
    <span>💿 Bandcamp</span>
</a>
<a href="https://www.facebook.com/tubanda" target="_blank" class="link-item">
    <span>📘 Facebook</span>
</a>
```

Puedes agregar tantos enlaces como necesites. Solo copia y pega el formato.

### 4️⃣ Cambiar el color del brillo (opcional)

Si quieres cambiar el brillo rojo a otro color:

**Busca en el CSS (líneas 56-58):**

```css
filter: drop-shadow(0 0 30px rgba(255, 0, 0, 0.5))
```

Cambia `rgba(255, 0, 0, 0.5)` por otro color:

- **Verde:** `rgba(0, 255, 0, 0.5)`
- **Azul:** `rgba(0, 100, 255, 0.5)`
- **Púrpura:** `rgba(150, 0, 255, 0.5)`
- **Blanco:** `rgba(255, 255, 255, 0.5)`

## 🌐 Cómo acceder a la página

### Opción 1: Como página principal

Renombra `band.html` a `index.html` (reemplaza el actual)

### Opción 2: Como página secundaria

Accede directamente a: `http://tudominio.com/band.html`

### Opción 3: Enlace desde index.html

Agrega un botón en tu `index.html` que lleve a `band.html`:

```html
<a href="band.html" class="btn-gradient">Ver Banda</a>
```

## 📱 Vista Previa

Para ver la página localmente, simplemente abre el archivo `band.html` en tu navegador.

## 🎭 Emojis disponibles para enlaces

- 🎵 Música
- 🎧 Streaming
- 📷 Fotos/Instagram
- 📘 Facebook
- 🎬 Videos
- 💿 Disco/Bandcamp
- 🎸 Guitarra
- 🥁 Batería
- 🎤 Micrófono
- 🔥 Fuego
- ⚡ Rayo
- 💀 Calavera
- 🖤 Corazón negro

## 💡 Consejos

1. **Logo:** Usa una imagen PNG con fondo transparente para mejor resultado
2. **Enlaces:** Asegúrate de que todas las URLs empiecen con `https://`
3. **Orden:** Los enlaces aparecen en el orden que los pongas en el código
4. **Prueba:** Revisa que todos los enlaces funcionen antes de publicar

## 🚀 Subir a InfinityFree

1. Conéctate a tu FTP (ftpupload.net)
2. Sube el archivo `band.html` a la carpeta `htdocs`
3. Si usas un logo, sube también la carpeta `img` con tu logo dentro
4. Accede a `http://tudominio.com/band.html`

## 🆘 Ayuda

Si necesitas ayuda para:

- Cambiar más colores
- Agregar más efectos
- Modificar animaciones
- Cualquier otra cosa

Solo pregúntame y te ayudaré! 🤘
