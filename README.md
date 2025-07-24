

---

```markdown
# Guía Paso a Paso: Creando tu Primera Landing Page Profesional

¡Bienvenido/a, futuro/a desarrollador/a!

En esta guía, vamos a construir desde cero una página de aterrizaje (landing page) completa y profesional para un producto ficticio llamado "Producto X". No solo aprenderás a escribir HTML y CSS, sino que también entenderás *por qué* estructuramos la página de una manera específica, utilizando el modelo de marketing **AIDA** (Atención, Interés, Deseo, Acción) para que sea efectiva.

**Tu Misión:** Seguir cada paso, escribir el código proporcionado y, lo más importante, entender qué hace cada parte. ¡Al final, tendrás un proyecto increíble para tu portafolio!

---

## Parte 1: La Preparación del Entorno

Todo gran proyecto empieza con una buena organización.

1.  **Crea la Carpeta del Proyecto:** En tu computadora, crea una carpeta nueva y llámala `landing-producto-x`.
2.  **Crea los Archivos Esenciales:** Dentro de esa carpeta, crea dos archivos vacíos:
    *   `index.html` (Aquí vivirá todo el contenido y la estructura).
    *   `style.css` (Aquí vivirá toda la magia del diseño y los colores).
3.  **Crea una Carpeta para Imágenes:** Dentro de `landing-producto-x`, crea otra carpeta y llámala `images`. Aquí guardarás todas las imágenes que uses.
4.  **Abre tu Editor de Código:** Abre la carpeta `landing-producto-x` completa con tu editor de código preferido (como Visual Studio Code).

---

## Parte 2: El Esqueleto de la Página (HTML Básico)

Vamos a darle a nuestro archivo `index.html` la estructura fundamental que toda página web necesita.

**➡️ Tu Tarea:** Copia el siguiente código y pégalo en tu archivo `index.html`.

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Producto X - La Solución Que Necesitas</title>
    
    <!-- Conectando nuestra hoja de estilos -->
    <link rel="stylesheet" href="style.css">

    <!-- Importando una fuente profesional desde Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- ¡Aquí construiremos toda nuestra página! -->
</body>
</html>
```

**💡 ¿Qué acabamos de hacer?**
*   **`<head>`**: Es la "mente" de la página. Contiene información importante (metadatos) pero no es visible.
*   **`<meta name="viewport"...>`**: Esencial para que tu página se vea bien en celulares.
*   **`<link rel="stylesheet" href="style.css">`**: La línea **más importante**. Conecta tu HTML con tu CSS. Sin esto, tu página no tendrá estilos.
*   **`<link href...>`**: Hemos importado la fuente "Poppins" de Google Fonts para que nuestra página tenga una tipografía moderna y legible.

---

## Parte 3: La Base del Diseño (CSS Global)

Antes de construir las secciones, definamos estilos generales que se aplicarán a toda la página. Esto nos ahorra trabajo y mantiene la consistencia.

**➡️ Tu Tarea:** Copia el siguiente código y pégalo en tu archivo `style.css`.

```css
/* ============================================ */
/*         ESTILOS GLOBALES Y VARIABLES         */
/* ============================================ */
:root {
    /* Usamos variables para poder cambiar los colores de toda la web desde un solo lugar */
    --primary-color: #0056b3; 
    --secondary-color: #007bff;
    --dark-color: #2c3e50;
    --light-color: #ecf0f1;
    --white-color: #ffffff;
    --font-family: 'Poppins', sans-serif;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box; /* Una regla clave para manejar tamaños de cajas más fácilmente */
}

html {
    scroll-behavior: smooth; /* Efecto de scroll suave al hacer clic en enlaces internos */
}

body {
    font-family: var(--font-family); /* Aplicamos la fuente que importamos */
    color: var(--dark-color);
    line-height: 1.6;
}

.container {
    max-width: 1100px; /* Limita el ancho del contenido para que no se estire demasiado en pantallas grandes */
    margin: 0 auto; /* Centra el contenedor */
    padding: 0 2rem;
}

h1, h2, h3 {
    line-height: 1.2;
    margin-bottom: 1rem;
}

h1 { font-size: 3rem; }
h2 { font-size: 2.5rem; color: var(--primary-color); text-align: center; margin-bottom: 3rem;}

section {
    padding: 5rem 0; /* Espaciado vertical entre secciones */
}

img {
    max-width: 100%; /* Asegura que las imágenes nunca se salgan de su contenedor */
    display: block;
}
```

**💡 ¿Qué acabamos de hacer?**
*   **Variables CSS (`:root`)**: Definimos nuestros colores principales. Si mañana quieres cambiar el azul por un verde, ¡solo lo cambias en un lugar!
*   **Reset (`*`)**: Eliminamos los márgenes y rellenos que los navegadores ponen por defecto.
*   **`.container`**: Creamos una clase "contenedora" que usaremos en cada sección para mantener el contenido centrado y ordenado.

---

## Parte 4: Construyendo la Página Sección por Sección

Ahora viene lo divertido. Añadiremos cada sección al `index.html` y su estilo correspondiente al `style.css`.

### Sección 1: El "Hero" (AIDA: Atención e Interés)

Esta es la primera impresión. Debe ser clara, potente y captar la **Atención** del usuario inmediatamente.

**➡️ Tu Tarea (Paso 1.1 - Contenido):**
1.  Busca en [Unsplash](https://unsplash.com/) una imagen que represente a tu "Producto X".
2.  Descárgala y guárdala en tu carpeta `images`. Renómbrala a algo sencillo, como `hero-image.jpg`.
3.  Copia el siguiente código HTML y pégalo **dentro** de la etiqueta `<body>` en tu `index.html`.

```html
<!-- ============================================ -->
<!--     SECCIÓN 1: HERO (Atención e Interés)     -->
<!-- ============================================ -->
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
            <!-- 👇 CAMBIA ESTA IMAGEN POR LA TUYA 👇 -->
            <img src="images/hero-image.jpg" alt="Persona usando el Producto X en una oficina moderna">
        </div>
    </div>
</header>

<main>
    <!-- El resto de las secciones irán dentro de <main> -->
```

**➡️ Tu Tarea (Paso 1.2 - Diseño):**
Ahora, hagamos que se vea bien. Copia este CSS y pégalo en tu archivo `style.css`.

```css
/* ============================================ */
/*                 ESTILOS DEL HERO             */
/* ============================================ */
.hero-section {
    background-color: var(--light-color);
    padding: 6rem 0;
}

.hero-content {
    display: flex; /* La magia de Flexbox: pone el texto y la imagen uno al lado del otro */
    align-items: center; /* Alinea verticalmente los elementos */
    gap: 3rem; /* Crea un espacio entre el texto y la imagen */
}

.hero-text { flex: 1; }
.hero-image { flex: 1; }

.hero-image img {
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1); /* Sombra sutil para darle profundidad */
}

.hero-text .subtitle { font-size: 1.2rem; margin-bottom: 2rem; }
.benefits .benefit-item { margin-bottom: 1rem; font-size: 1.1rem; }

/* Estilo para nuestro botón principal de llamada a la acción (CTA) */
.cta-button {
    display: inline-block;
    background-color: var(--secondary-color);
    color: var(--white-color);
    padding: 1rem 2rem;
    border-radius: 5px;
    text-decoration: none;
    font-weight: 600;
    margin-top: 1.5rem;
    transition: background-color 0.3s ease, transform 0.3s ease; /* Transición suave */
}

.cta-button:hover {
    background-color: var(--primary-color);
    transform: translateY(-3px); /* Efecto de "levantarse" al pasar el ratón */
}
```

**✅ ¡Revisa tu Progreso!**
Guarda ambos archivos y abre `index.html` en tu navegador. ¡Ya deberías ver tu increíble sección Hero!

---

### Sección 2: Testimonios (AIDA: Interés y Deseo)

La prueba social es muy poderosa. Mostrar que otras personas confían en tu producto genera **Interés** y **Deseo**.

**➡️ Tu Tarea (Paso 2.1 - Contenido):**
1.  Para las fotos de los testimonios, puedes usar [Random User Generator](https://randomuser.me/) o buscar fotos de personas en Unsplash.
2.  Copia el siguiente código HTML y pégalo **dentro** de la etiqueta `<main>` en tu `index.html`.

```html
<!-- ============================================ -->
<!--    SECCIÓN 2: TESTIMONIOS (Interés y Deseo)  -->
<!-- ============================================ -->
<section id="testimonials" class="testimonials-section">
    <div class="container">
        <h2>Lo que dicen nuestros clientes</h2>
        <div class="testimonials-grid">
            <!-- Testimonio 1 -->
            <div class="testimonial-card">
                <img src="https://randomuser.me/api/portraits/women/32.jpg" alt="Foto de Ana García" class="testimonial-avatar">
                <blockquote>"Producto X cambió las reglas del juego para mi equipo. ¡Increíble!"</blockquote>
                <cite>– Ana García, Gerente de Proyectos</cite>
            </div>
            
            <!-- Testimonio 2 -->
            <div class="testimonial-card">
                <img src="https://randomuser.me/api/portraits/men/45.jpg" alt="Foto de Carlos Rodriguez" class="testimonial-avatar">
                <blockquote>"Era escéptico al principio, pero la facilidad de uso me convenció."</blockquote>
                <cite>– Carlos Rodríguez, Desarrollador Freelance</cite>
            </div>

            <!-- Testimonio 3 -->
            <div class="testimonial-card">
                <img src="https://randomuser.me/api/portraits/women/50.jpg" alt="Foto de Laura Fernandez" class="testimonial-avatar">
                <blockquote>"El aumento en la productividad fue evidente desde la primera semana."</blockquote>
                <cite>– Laura Fernández, Directora de Operaciones</cite>
            </div>
        </div>
    </div>
</section>
```

**➡️ Tu Tarea (Paso 2.2 - Diseño):**
Vamos a usar `Grid` para alinear las tarjetas de testimonio perfectamente. Copia este CSS en `style.css`.

```css
/* ============================================ */
/*              ESTILOS TESTIMONIOS             */
/* ============================================ */
.testimonials-section {
    background-color: var(--white-color);
}

.testimonials-grid {
    display: grid; /* Usamos Grid para crear una cuadrícula flexible */
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); /* ¡Magia responsiva! */
    gap: 2rem;
}

/* 
   Explicación de la línea mágica de Grid:
   - "repeat(auto-fit, ...)" : Crea tantas columnas como quepan en el contenedor.
   - "minmax(300px, 1fr)" : Cada columna tendrá un mínimo de 300px y se estirará para ocupar el espacio sobrante (1fr).
   Esto hace que en pantallas grandes se vean 3 columnas, y en móviles se apilen una sobre otra automáticamente.
*/

.testimonial-card {
    background: var(--light-color);
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    text-align: center;
}

.testimonial-avatar {
    width: 80px;
    height: 80px;
    border-radius: 50%; /* La clave para hacer imágenes redondas */
    margin: 0 auto 1rem;
    border: 3px solid var(--secondary-color);
}

.testimonial-card blockquote { font-style: italic; margin-bottom: 1rem; font-size: 1.1rem; }
.testimonial-card cite { font-weight: 600; color: var(--primary-color); }
```

**✅ ¡Revisa tu Progreso!**
Guarda y refresca el navegador. Deberías ver tus testimonios en una cuadrícula perfecta. ¡Intenta cambiar el tamaño de la ventana del navegador para ver la magia responsiva en acción!

---

### Sección 3: Galería de Producto (AIDA: Deseo)

Mostrar el producto en acción es clave para despertar el **Deseo** de tenerlo.

**➡️ Tu Tarea (Paso 3.1 - Contenido):**
1.  Busca 4 imágenes en Unsplash que muestren tu producto. Guárdalas en tu carpeta `images`.
2.  Copia el siguiente HTML y pégalo en `index.html`, justo después de la sección de testimonios.

```html
<!-- ============================================ -->
<!--     SECCIÓN 3: GALERÍA (Deseo)               -->
<!-- ============================================ -->
<section id="gallery" class="gallery-section">
    <div class="container">
        <h2>Explora Producto X en Acción</h2>
        <div class="gallery-grid">
            <!-- 👇 CAMBIA ESTAS IMÁGENES POR LAS TUYAS 👇 -->
            <img src="images/gallery-1.jpg" alt="Interfaz del Producto X mostrando un dashboard">
            <img src="images/gallery-2.jpg" alt="Equipo colaborando con el Producto X">
            <img src="images/gallery-3.jpg" alt="Gráficos y analíticas generadas por el Producto X">
            <img src="images/gallery-4.jpg" alt="Integración del Producto X con otras herramientas">
        </div>
    </div>
</section>
```

**➡️ Tu Tarea (Paso 3.2 - Diseño):**
Usaremos `Grid` de nuevo para crear un mosaico de imágenes perfecto. Copia este CSS en `style.css`.

```css
/* ============================================ */
/*                ESTILOS GALERÍA               */
/* ============================================ */
.gallery-section {
    background-color: var(--light-color);
}

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* Crea una cuadrícula de 2x2 */
    gap: 1.5rem;
}

.gallery-grid img {
    width: 100%;
    height: 100%;
    object-fit: cover; /* Asegura que la imagen cubra todo el espacio sin deformarse */
    border-radius: 8px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
}

.gallery-grid img:hover {
    transform: scale(1.05); /* Agranda la imagen ligeramente al pasar el ratón */
}
```

---

### Secciones 4 y 5: FAQ y Formulario (AIDA: Deseo y Acción)

Resolvemos las últimas dudas (Deseo) y le damos al usuario un camino claro para el siguiente paso (**Acción**).

**➡️ Tu Tarea (Paso 4.1 - Contenido):**
Copia el HTML para las dos secciones siguientes y pégalo en `index.html`.

```html
<!-- ============================================ -->
<!-- SECCIÓN 4: PREGUNTAS FRECUENTES (Deseo/Acción) -->
<!-- ============================================ -->
<section id="faq" class="faq-section">
    <div class="container">
        <h2>Preguntas Frecuentes</h2>
        <div class="faq-container">
            <div class="faq-item">
                <h3 class="faq-question">¿Necesito conocimientos técnicos para usar Producto X?</h3>
                <p class="faq-answer">No, en absoluto. Producto X está diseñado con una interfaz muy intuitiva.</p>
            </div>
            <div class="faq-item">
                <h3 class="faq-question">¿Qué tipo de soporte ofrecen?</h3>
                <p class="faq-answer">Ofrecemos soporte 24/7 a través de chat en vivo y correo electrónico.</p>
            </div>
        </div>
    </div>
</section>

<!-- ============================================ -->
<!--     SECCIÓN 5: FORMULARIO (Acción)           -->
<!-- ============================================ -->
<section id="contact" class="contact-section">
    <div class="container">
        <h2>¿Listo para empezar?</h2>
        <p>Déjanos tus datos y un especialista se pondrá en contacto contigo.</p>
        <form class="contact-form" action="#" method="POST">
            <input type="text" name="name" placeholder="Tu Nombre Completo" required>
            <input type="email" name="email" placeholder="Tu Correo Electrónico" required>
            <textarea name="message" rows="4" placeholder="Cuéntanos un poco sobre tus necesidades (opcional)"></textarea>
            <button type="submit" class="cta-button">Enviar Información</button>
        </form>
    </div>
</section>
```

**➡️ Tu Tarea (Paso 4.2 - Diseño):**
Finalmente, añade los estilos para estas dos secciones en tu archivo `style.css`.

```css
/* ============================================ */
/*                  ESTILOS FAQ                 */
/* ============================================ */
.faq-section { background-color: var(--white-color); }
.faq-container { max-width: 800px; margin: 0 auto; }
.faq-item { border-bottom: 1px solid #ccc; padding-bottom: 1.5rem; margin-bottom: 1.5rem; }
.faq-item:last-child { border-bottom: none; }
.faq-question { color: var(--primary-color); margin-bottom: 0.5rem; }

/* ============================================ */
/*               ESTILOS CONTACTO               */
/* ============================================ */
.contact-section {
    background-color: var(--dark-color);
    color: var(--white-color);
    text-align: center;
}
.contact-section h2 { color: var(--white-color); }
.contact-form {
    max-width: 600px;
    margin: 2rem auto 0;
    display: flex;
    flex-direction: column; /* Apila los campos del formulario verticalmente */
    gap: 1rem;
}
.contact-form input,
.contact-form textarea {
    width: 100%;
    padding: 1rem;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-family: var(--font-family);
    font-size: 1rem;
}
.contact-form button { width: 100%; cursor: pointer; border: none; }
```
---

## Parte 5: El Toque Final (Footer y Diseño Responsivo)

Toda página necesita un pie de página y debemos asegurarnos de que se vea perfecta en móviles.

**➡️ Tu Tarea (Paso 5.1 - Contenido):**
Cierra la etiqueta `<main>` y añade el `<footer>` al final de tu `index.html`, justo antes de cerrar `</body>`.

```html
<!-- Pega esto después de la etiqueta </main> -->
</main>

<footer class="footer">
    <div class="container">
        <p>&copy; 2024 Producto X. Todos los derechos reservados.</p>
    </div>
</footer>
```

**➡️ Tu Tarea (Paso 5.2 - Diseño):**
Añade los últimos estilos para el footer y, lo más importante, las **Media Queries** para el diseño responsivo en `style.css`.

```css
/* ============================================ */
/*               ESTILOS FOOTER                 */
/* ============================================ */
.footer {
    background: var(--light-color);
    text-align: center;
    padding: 2rem 0;
    font-size: 0.9rem;
}

/* ============================================ */
/*             DISEÑO RESPONSIVO                */
/* ============================================ */
@media(max-width: 768px) {
    h1 { font-size: 2.2rem; }
    h2 { font-size: 2rem; }

    /* Hacemos que el Hero se apile en pantallas pequeñas */
    .hero-content {
        flex-direction: column; /* Cambia la dirección de flex a vertical */
        text-align: center;
    }
    
    .hero-text { order: 2; } /* Pone el texto debajo de la imagen */
    .hero-image { order: 1; } /* Pone la imagen arriba */

    /* Hacemos que la galería sea de una sola columna */
    .gallery-grid {
        grid-template-columns: 1fr;
    }
}
```

**💡 ¿Qué es `@media`?**
Es una regla de CSS que aplica estilos solo si se cumple una condición. En este caso, `@media(max-width: 768px)` significa: "Aplica los siguientes estilos ÚNICAMENTE si el ancho de la pantalla es de 768px o menos (es decir, tablets y móviles)".

---

## 🚀 ¡Felicidades! 🚀

¡Lo has logrado! Guarda todos tus archivos y abre `index.html` en tu navegador. Deberías tener una landing page completa, moderna y profesional.

### Para probar el diseño responsivo:
1.  Abre las herramientas de desarrollador en tu navegador (usualmente con la tecla `F12` o `Cmd+Option+I` en Mac).
2.  Busca un ícono que se parezca a un teléfono y una tablet (Toggle device toolbar).
3.  Juega con los diferentes tamaños de pantalla para ver cómo tu diseño se adapta perfectamente.

¡Este es un proyecto fantástico para tu portafolio y un gran paso en tu carrera como desarrollador/a!
```
