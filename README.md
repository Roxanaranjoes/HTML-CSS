# Learning HTML & CSS 🌐

This repository is my personal space where I'm documenting my learning journey with HTML and CSS.

Here, I'm saving exercises, practice files, and small projects that I’m building as I learn from scratch.

✨ **Why this repo?**

Because I want to see my progress, practice what I learn, and keep everything organized. 

## 📚 What you’ll find here

- Basic HTML and CSS exercises
- Layout practice (Flexbox, Grid)
- Responsive design examples
- Small practice projects
- My notes and experiments

## 👩‍💻 Author

**Roxana Naranjo Estrada**  
Learning HTML and CSS from scratch with dedication and excitement 💪

---

Thanks for visiting my repository 😊/
* Teléfonos pequeños (0–480px) */
@media (max-width: 480px) {
  body {
    background-color: lightcoral;
  }
}

/* Teléfonos grandes y tablets pequeñas (481–768px) */
@media (min-width: 481px) and (max-width: 768px) {
  body {
    background-color: lightblue;
  }
}

/* Tablets y laptops pequeñas (769–1024px) */
@media (min-width: 769px) and (max-width: 1024px) {
  body {
    background-color: lightgreen;
  }
}

/* Laptops y escritorios grandes (1025px en adelante) */
@media (min-width: 1025px) {
  body {
    background-color: lightgray;
  }
}
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mi Sitio Semántico</title>
  <link rel="stylesheet" href="css/style.css" />
</head>
<body>

  <header>
    <nav>
      <ul>
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#sobre-mi">Sobre mí</a></li>
        <li><a href="#proyectos">Proyectos</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <main>

    <section id="inicio">
      <h1>Bienvenid@ a mi sitio web</h1>
      <p>Este es un ejemplo de HTML semántico.</p>
    </section>

    <section id="sobre-mi">
      <h2>Sobre mí</h2>
      <p>Soy desarrolladora web con pasión por el diseño y la accesibilidad.</p>
    </section>

    <section id="proyectos">
      <h2>Proyectos destacados</h2>
      <article>
        <h3>Proyecto 1</h3>
        <p>Descripción breve del proyecto.</p>
      </article>
      <article>
        <h3>Proyecto 2</h3>
        <p>Descripción breve del proyecto.</p>
      </article>
    </section>

    <section id="contacto">
      <h2>Contacto</h2>
      <form>
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" required />

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required />

        <label for="mensaje">Mensaje:</label>
        <textarea id="mensaje" name="mensaje" required></textarea>

        <button type="submit">Enviar</button>
      </form>
    </section>

  </main>

  <footer>
    <p>&copy; 2025 Tu Nombre. Todos los derechos reservados.</p>
  </footer>

</body>
</html>

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mi Portafolio | Roxana Naranjo</title>
  <link rel="stylesheet" href="styles/styles.css" />
</head>
<body>
  <header>
    <h1>Roxana Naranjo</h1>
    <nav>
      <ul>
        <li><a href="about.html">Sobre mí</a></li>
        <li><a href="portfolio.html">Portafolio</a></li>
        <li><a href="contact.html">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="intro">
      <h2>Bienvenidos</h2>
      <p>Desarrolladora web con pasión por el diseño, la tecnología y las experiencias digitales significativas.</p>
    </section>
  </main>

  <footer>
    <p>© 2025 Roxana Naranjo. Todos los derechos reservados.</p>
  </footer>
</body>
</html>
/* Tipografía y colores base */
body {
  font-family: 'Segoe UI', sans-serif;
  margin: 0;
  background: #f2f2f2;
  color: #333;
  line-height: 1.6;
}

header, nav, footer {
  background-color: #0077b6;
  color: white;
  padding: 1rem;
}

nav ul {
  display: flex;
  gap: 1rem;
  list-style: none;
  justify-content: center;
}

nav a {
  color: white;
  text-decoration: none;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #90e0ef;
}

/* Secciones principales */
main {
  padding: 2rem;
}

.intro {
  text-align: center;
  background-color: white;
  padding: 2rem;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.intro:hover {
  transform: translateY(-5px);
}

/* Diseño Responsivo */
@media (max-width: 1024px) {
  nav ul {
    flex-direction: column;
  }
}

@media (max-width: 768px) {
  .intro {
    padding: 1rem;
  }
}

@media (max-width: 480px) {
  header, nav, footer {
    text-align: center;
  }
}

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Portafolio | Roxana</title>
  <link rel="stylesheet" href="styles/styles.css" />
</head>
<body>
  <header>
    <h1>Mi Portafolio</h1>
    <nav>
      <ul>
        <li><a href="index.html">Inicio</a></li>
        <li><a href="about.html">Sobre mí</a></li>
        <li><a href="contact.html">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="portfolio-grid">
      <article class="project">
        <img src="images/proyecto1.jpg" alt="Proyecto 1" />
        <h3>Proyecto 1</h3>
        <p>Sitio web para una tienda de ropa ecológica.</p>
      </article>
      <article class="project">
        <img src="images/proyecto2.jpg" alt="Proyecto 2" />
        <h3>Proyecto 2</h3>
        <p>Blog personal sobre viajes y cultura.</p>
      </article>
      <article class="project">
        <img src="images/proyecto3.jpg" alt="Proyecto 3" />
        <h3>Proyecto 3</h3>
        <p>Plataforma de recetas veganas.</p>
      </article>
    </section>
  </main>

  <footer>
    <p>Gracias por visitar mi portafolio.</p>
  </footer>
</body>
</html>
.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
}

.project {
  background: white;
  padding: 1rem;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.project:hover {
  transform: scale(1.03);
}

.project img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
}
# Portafolio Web – Roxana Naranjo

## Descripción
Este sitio web es un portafolio personal donde presento quién soy, algunos de mis proyectos y una forma de contactarme.

## Estructura
- **index.html:** Página principal
- **about.html:** Sobre mí
- **portfolio.html:** Proyectos destacados
- **contact.html:** Formulario de contacto

## Tecnologías
- HTML5
- CSS3 (Flexbox + Grid)
- Diseño Responsivo

## Información del Coder
- **Nombre:** Roxana Naranjo Estrada
- **Clan:** Be a Codernnn
- **Correo:** roxana@example.com
- **Documento de Identidad:** 123456789

## Cómo visualizar el proyecto
Puedes clonar el repositorio y abrir `index.html` en tu navegador favorito.
//github.com/jmgrgo/developmentTraining_Riwi/tree/main/Module2/additionalExercises/Positivus
