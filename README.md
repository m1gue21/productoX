
---

# **Guía Paso a Paso: Creando una Landing Page Completa con HTML y CSS**

**Objetivo del Proyecto:** Construir una landing page profesional y atractiva para un producto ficticio ("Producto X"). Aprenderás a estructurar contenido con HTML5 semántico y a darle estilo con CSS, utilizando técnicas modernas como Flexbox y Grid. Además, aplicaremos el modelo de marketing **AIDA** para que la página no solo sea bonita, sino también efectiva.

### **¿Qué es el modelo AIDA?**

Es una fórmula clásica de marketing que guía al usuario a través de un proceso de compra:

*   **A - Atención:** Captar la mirada del visitante en los primeros segundos.
*   **I - Interés:** Generar curiosidad y hacer que quieran saber más.
*   **D - Deseo:** Convencerlos de que tu producto es la solución que necesitan.
*   **A - Acción:** Incitarlos a realizar una acción concreta (comprar, registrarse, etc.).

Nuestra página se estructurará así:
1.  **Hero:** Atención e Interés.
2.  **Testimonios:** Interés y Deseo.
3.  **Galería:** Deseo.
4.  **FAQ:** Apoya el Deseo y prepara la Acción.
5.  **Formulario:** Acción.

---

### **Paso 0: Preparación del Entorno**

Antes de escribir código, necesitas organizar tu espacio de trabajo.

1.  **Crea una carpeta:** En tu escritorio o donde prefieras, crea una carpeta nueva y llámala `mi-landing-page`.
2.  **Crea los archivos:** Dentro de esa carpeta, crea dos archivos:
    *   `index.html` (aquí vivirá la estructura de tu página).
    *   `style.css` (aquí escribirás todas las reglas de estilo).
3.  **Abre la carpeta en tu editor de código:** Usa un editor como Visual Studio Code, Sublime Text o Atom. Abre la carpeta `mi-landing-page` completa para tener acceso fácil a ambos archivos.

---

### **Paso 1: La Estructura Base (HTML)**

En tu archivo `index.html`, vamos a empezar con la estructura básica de cualquier página web.

**Tu Tarea:**
Copia y pega este código en tu archivo `index.html`.

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Producto X - La Solución Que Necesitas</title>
    <!-- Aquí conectamos nuestro archivo CSS -->
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Todo el contenido de nuestra página irá aquí -->
</body>
</html>
```

**Explicación:**
*   `<!DOCTYPE html>`: Define el tipo de documento.
*   `<meta charset="UTF-8">`: Asegura que el navegador muestre correctamente caracteres especiales como tildes y "ñ".
*   `<meta name="viewport"...>`: Es **crucial** para el diseño responsivo. Hace que la página se adapte al ancho del dispositivo (móvil, tablet, etc.).
*   `<link rel="stylesheet" href="style.css">`: Esta es la línea mágica que conecta tu HTML con tu hoja de estilos CSS. **Sin ella, tus estilos no se aplicarán.**

---

### **Paso 2: Creando las Secciones (Una por una)**

Ahora iremos construyendo cada sección dentro de la etiqueta `<body>`.

#### **Sección 1: El Hero (Atención e Interés)**

Esta es la primera impresión. Debe ser impactante.

**Tu Tarea:**
1.  **Inventa tu Producto X:** ¿Qué hace? ¿A quién ayuda? Sé creativo.
2.  **Busca una imagen principal:** Ve a sitios como [Unsplash](https://unsplash.com/) o [Pexels](https://www.pexels.com/es-es/) y busca una imagen que represente tu producto. Descárgala y guárdala en tu carpeta `mi-landing-page` (puedes crear una subcarpeta llamada `images`).
3.  **Escribe el código:** Dentro del `<body>`, añade el siguiente código HTML. Reemplaza los textos y el `src` de la imagen con tu propio contenido.

```html
<!-- Pega esto dentro de <body> -->
<header class="hero-section">
    <div class="container hero-content">
        <div class="hero-text">
            <h1>Descubre Producto X: Transforma tu día a día</h1>
            <p class="subtitle">La herramienta definitiva que simplifica tus tareas complejas y te devuelve tu tiempo más valioso.</p>
            
            <div class="benefits">
                <div class="benefit-item"><strong>✅ Eficiencia Máxima:</strong> Ahorra hasta un 50% de tiempo.</div>
                <div class="benefit-item"><strong>✅ Fácil de Usar:</strong> Interfaz intuitiva.</div>
                <div class="benefit-item"><strong>✅ Resultados Garantizados:</strong> Únete a miles de usuarios.</div>
            </div>
            
            <a href="#contact" class="cta-button">¡Quiero saber más!</a>
        </div>
        <div class="hero-image">
            <!-- Cambia "tu-imagen-principal.jpg" por el nombre de tu archivo -->
            <img src="images/tu-imagen-principal.jpg" alt="Persona usando el Producto X">
        </div>
    </div>
</header>
```

**Ahora, dale estilo en `style.css`:**

```css
/* Pega esto en style.css */
.hero-section {
    background-color: #ecf0f1; /* Un gris claro de fondo */
    padding: 6rem 0;
}

.hero-content {
    display: flex; /* ¡Magia! Pone el texto y la imagen uno al lado del otro */
    align-items: center; /* Los alinea verticalmente */
    gap: 3rem; /* Crea un espacio entre el texto y la imagen */
}

.hero-text { flex: 1; }
.hero-image { flex: 1; }

.hero-image img {
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
}

/* Y no olvides el botón! */
.cta-button {
    display: inline-block;
    background-color: #007bff;
    color: #ffffff;
    padding: 1rem 2rem;
    border-radius: 5px;
    text-decoration: none;
    font-weight: 600;
    margin-top: 1.5rem;
}
```
**Explicación del CSS:**
*   `display: flex;` es una de las herramientas más potentes de CSS para alinear elementos. Convierte a `.hero-content` en un "contenedor flexible".
*   `flex: 1;` le dice a los hijos (`.hero-text` y `.hero-image`) que compartan el espacio disponible por igual.

*(Continúa este patrón para cada una de las secciones: Testimonios, Galería, FAQ y Formulario. En cada paso, explica la tarea del estudiante, proporciona el bloque de HTML, el bloque de CSS correspondiente y una breve explicación de las propiedades clave que se están utilizando, como `display: grid` para la galería o `flex-direction: column` para el formulario).*

---

### **Paso 3: Uniendo Todo y Siguientes Pasos**

Una vez que hayas añadido todas las secciones y sus estilos, ¡es hora de ver tu creación!

1.  **Abre el archivo `index.html` en tu navegador:** Ve a tu carpeta `mi-landing-page`, haz clic derecho en `index.html` y selecciona "Abrir con" -> "Google Chrome" (o tu navegador preferido).
2.  **Revisa y ajusta:** ¿Se ve todo como esperabas? ¿Los colores combinan? ¿Los textos son legibles? Este es el momento de volver a tu archivo `style.css` y hacer pequeños ajustes en los colores, tamaños de fuente, espaciados, etc.

**¡Felicidades!** Has construido una landing page completa y funcional.

### **Desafíos Adicionales (Para seguir aprendiendo):**

*   **Añade interactividad al FAQ:** Investiga cómo usar un poco de JavaScript para que las respuestas del FAQ se muestren y oculten al hacer clic en las preguntas (esto se llama "acordeón").
*   **Anima los elementos:** Usa transiciones (`transition`) y transformaciones (`transform`) de CSS para que los elementos aparezcan suavemente al hacer scroll o para que los botones tengan un efecto más dinámico al pasar el ratón por encima.
*   **Personaliza la fuente:** Ve a [Google Fonts](https://fonts.google.com/), elige una tipografía que te guste e impleméntala en tu proyecto (ya hemos dejado la base en el `<head>` del HTML).
