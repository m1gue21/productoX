---

### **Fase 1: Código Completo del Proyecto**

Aquí tienes los dos archivos, `index.html` y `style.css`, que conforman la landing page. El código está diseñado para ser moderno, responsivo y fácil de entender.

#### **Archivo: `index.html`**

Este archivo contiene la estructura semántica de la página.

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Producto X - La Solución Que Necesitas</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>

    <!-- ============================================ -->
    <!--     SECCIÓN 1: HERO (Atención e Interés)     -->
    <!-- ============================================ -->
    <header class="hero-section">
        <div class="container hero-content">
            <div class="hero-text">
                <h1>Descubre Producto X: Transforma tu día a día</h1>
                <p class="subtitle">La herramienta definitiva que simplifica tus tareas complejas y te devuelve tu tiempo más valioso.</p>
                
                <div class="benefits">
                    <div class="benefit-item">
                        <strong>✅ Eficiencia Máxima:</strong> Ahorra hasta un 50% de tiempo en tus procesos diarios.
                    </div>
                    <div class="benefit-item">
                        <strong>✅ Fácil de Usar:</strong> Interfaz intuitiva diseñada para que empieces a usarlo en minutos.
                    </div>
                    <div class="benefit-item">
                        <strong>✅ Resultados Garantizados:</strong> Únete a miles de usuarios satisfechos que ya han mejorado su productividad.
                    </div>
                </div>
                
                <a href="#contact" class="cta-button">¡Quiero saber más!</a>
            </div>
            <div class="hero-image">
                <!-- El estudiante debe reemplazar esta imagen -->
                <img src="https://images.unsplash.com/photo-1556740738-b6a63e27c4df?q=80&w=2070" alt="Persona usando el Producto X en una oficina moderna">
            </div>
        </div>
    </header>

    <main>
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
                        <blockquote>
                            "Producto X cambió las reglas del juego para mi equipo. Lo que antes nos tomaba horas, ahora lo hacemos en minutos. ¡Increíble!"
                        </blockquote>
                        <cite>– Ana García, Gerente de Proyectos</cite>
                    </div>
                    
                    <!-- Testimonio 2 -->
                    <div class="testimonial-card">
                        <img src="https://randomuser.me/api/portraits/men/45.jpg" alt="Foto de Carlos Rodriguez" class="testimonial-avatar">
                        <blockquote>
                            "Era escéptico al principio, pero la facilidad de uso y el soporte al cliente me convencieron. Totalmente recomendado."
                        </blockquote>
                        <cite>– Carlos Rodríguez, Desarrollador Freelance</cite>
                    </div>

                    <!-- Testimonio 3 -->
                    <div class="testimonial-card">
                        <img src="https://randomuser.me/api/portraits/women/50.jpg" alt="Foto de Laura Fernandez" class="testimonial-avatar">
                        <blockquote>
                            "Implementamos Producto X en toda la empresa y el aumento en la productividad fue evidente desde la primera semana. Una inversión que vale la pena."
                        </blockquote>
                        <cite>– Laura Fernández, Directora de Operaciones</cite>
                    </div>
                </div>
            </div>
        </section>

        <!-- ============================================ -->
        <!--     SECCIÓN 3: GALERÍA (Deseo)               -->
        <!-- ============================================ -->
        <section id="gallery" class="gallery-section">
            <div class="container">
                <h2>Explora Producto X en Acción</h2>
                <div class="gallery-grid">
                    <!-- El estudiante debe reemplazar estas imágenes -->
                    <img src="https://images.unsplash.com/photo-1587620962725-abab7fe55159?q=80&w=1931" alt="Interfaz del Producto X mostrando un dashboard">
                    <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?q=80&w=2070" alt="Equipo colaborando con el Producto X">
                    <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?q=80&w=2070" alt="Gráficos y analíticas generadas por el Producto X">
                    <img src="https://images.unsplash.com/photo-1516321497487-e288fb19713f?q=80&w=2070" alt="Integración del Producto X con otras herramientas">
                </div>
            </div>
        </section>

        <!-- ============================================ -->
        <!-- SECCIÓN 4: PREGUNTAS FRECUENTES (Deseo/Acción) -->
        <!-- ============================================ -->
        <section id="faq" class="faq-section">
            <div class="container">
                <h2>Preguntas Frecuentes</h2>
                <div class="faq-container">
                    <div class="faq-item">
                        <h3 class="faq-question">¿Necesito conocimientos técnicos para usar Producto X?</h3>
                        <p class="faq-answer">No, en absoluto. Producto X está diseñado con una interfaz muy intuitiva. Si sabes usar un navegador web, puedes usar nuestra herramienta sin problemas.</p>
                    </div>
                    <div class="faq-item">
                        <h3 class="faq-question">¿Qué tipo de soporte ofrecen?</h3>
                        <p class="faq-answer">Ofrecemos soporte 24/7 a través de chat en vivo y correo electrónico. Además, nuestros planes premium incluyen un gestor de cuenta dedicado.</p>
                    </div>
                    <div class="faq-item">
                        <h3 class="faq-question">¿Hay un período de prueba gratuito?</h3>
                        <p class="faq-answer">¡Sí! Puedes probar todas las funcionalidades de Producto X durante 14 días, sin compromiso y sin necesidad de tarjeta de crédito.</p>
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
    </main>

    <footer class="footer">
        <div class="container">
            <p>&copy; 2024 Producto X. Todos los derechos reservados.</p>
        </div>
    </footer>

</body>
</html>
```

#### **Archivo: `style.css`**

Este archivo contiene todos los estilos para dar vida al HTML.

```css
/* ============================================ */
/*         ESTILOS GLOBALES Y VARIABLES         */
/* ============================================ */
:root {
    --primary-color: #0056b3; /* Un azul corporativo fuerte */
    --secondary-color: #007bff; /* Un azul más brillante para acentos */
    --dark-color: #2c3e50; /* Gris oscuro para texto */
    --light-color: #ecf0f1; /* Gris muy claro para fondos */
    --white-color: #ffffff;
    --font-family: 'Poppins', sans-serif;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth; /* Desplazamiento suave al hacer clic en enlaces */
}

body {
    font-family: var(--font-family);
    color: var(--dark-color);
    line-height: 1.6;
}

.container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 2rem;
}

h1, h2, h3 {
    line-height: 1.2;
    margin-bottom: 1rem;
}

h1 { font-size: 3rem; }
h2 { font-size: 2.5rem; color: var(--primary-color); text-align: center; margin-bottom: 3rem;}
h3 { font-size: 1.5rem; }

section {
    padding: 5rem 0;
}

img {
    max-width: 100%;
    display: block;
}

/* ============================================ */
/*              ESTILOS DEL BOTÓN CTA           */
/* ============================================ */
.cta-button {
    display: inline-block;
    background-color: var(--secondary-color);
    color: var(--white-color);
    padding: 1rem 2rem;
    border-radius: 5px;
    text-decoration: none;
    font-weight: 600;
    margin-top: 1.5rem;
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.cta-button:hover {
    background-color: var(--primary-color);
    transform: translateY(-3px);
}

/* ============================================ */
/*                 ESTILOS DEL HERO             */
/* ============================================ */
.hero-section {
    background-color: var(--light-color);
    padding: 6rem 0;
}

.hero-content {
    display: flex;
    align-items: center;
    gap: 3rem;
}

.hero-text {
    flex: 1; /* Ocupa el espacio disponible */
}

.hero-text .subtitle {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.benefits .benefit-item {
    margin-bottom: 1rem;
    font-size: 1.1rem;
}

.hero-image {
    flex: 1;
}

.hero-image img {
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
}

/* ============================================ */
/*              ESTILOS TESTIMONIOS             */
/* ============================================ */
.testimonials-section {
    background-color: var(--white-color);
}

.testimonials-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

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
    border-radius: 50%;
    margin: 0 auto 1rem;
    border: 3px solid var(--secondary-color);
}

.testimonial-card blockquote {
    font-style: italic;
    margin-bottom: 1rem;
    font-size: 1.1rem;
}

.testimonial-card cite {
    font-weight: 600;
    color: var(--primary-color);
}

/* ============================================ */
/*                ESTILOS GALERÍA               */
/* ============================================ */
.gallery-section {
    background-color: var(--light-color);
}

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
}

.gallery-grid img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 8px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
}

.gallery-grid img:hover {
    transform: scale(1.05);
}

/* ============================================ */
/*                  ESTILOS FAQ                 */
/* ============================================ */
.faq-section {
    background-color: var(--white-color);
}

.faq-container {
    max-width: 800px;
    margin: 0 auto;
}

.faq-item {
    border-bottom: 1px solid #ccc;
    padding-bottom: 1.5rem;
    margin-bottom: 1.5rem;
}

.faq-item:last-child {
    border-bottom: none;
}

.faq-question {
    color: var(--primary-color);
    margin-bottom: 0.5rem;
}

/* ============================================ */
/*               ESTILOS CONTACTO               */
/* ============================================ */
.contact-section {
    background-color: var(--dark-color);
    color: var(--white-color);
    text-align: center;
}

.contact-section h2 {
    color: var(--white-color);
}

.contact-form {
    max-width: 600px;
    margin: 2rem auto 0;
    display: flex;
    flex-direction: column;
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

.contact-form button {
    width: 100%;
    cursor: pointer;
    border: none;
}

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

    /* Hero responsivo */
    .hero-content {
        flex-direction: column;
        text-align: center;
    }
    
    .hero-text {
        order: 2; /* Pone el texto debajo de la imagen */
    }

    .hero-image {
        order: 1; /* Pone la imagen arriba */
    }

    /* Galería responsiva */
    .gallery-grid {
        grid-template-columns: 1fr;
    }
}
```

---

### **Fase 2: Guía Paso a Paso para el Estudiante (Formato para Word)**

Aquí tienes el contenido para el documento de Word.

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
