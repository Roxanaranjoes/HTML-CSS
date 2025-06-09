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

https://github.com/jmgrgo/developmentTraining_Riwi/tree/main/Module2/additionalExercises/Positivus
