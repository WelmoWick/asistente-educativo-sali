<template>
  <div id="app">
    <header class="top-bar">
      <nav>
        <ul class="nav-links">
          <li>
            <a
              href="https://drive.google.com"
              target="_blank"
              rel="noopener noreferrer"
              class="nav-link"
            >
              Drive
            </a>
          </li>
          <li>
            <a
              href="https://wa.me/573001112233"
              target="_blank"
              rel="noopener noreferrer"
              class="nav-link"
            >
              WhatsApp
            </a>
          </li>
        </ul>
      </nav>
    </header>
    <main class="content">
      <h1>SALI – Asistente Educativo</h1>
      <section>
        <h2>¿Qué es SALI?</h2>
        <p>SALI es un asistente virtual inteligente creado para colegios. Utiliza inteligencia artificial para responder preguntas frecuentes sobre horarios, matrículas, reuniones, eventos y más, reduciendo hasta un 80&nbsp;% la carga administrativa.</p>
      </section>
      <section>
        <h2>Objetivo</h2>
        <p>Modernizar los procesos administrativos escolares, aliviando el trabajo de la secretaría y mejorando la experiencia de padres y estudiantes mediante la automatización de consultas y solicitudes básicas.</p>
      </section>
      <section>
        <h2>Funcionalidades principales</h2>
        <ul>
          <li>Responde preguntas frecuentes de la comunidad educativa.</li>
          <li>Informa sobre fechas académicas y reuniones escolares.</li>
          <li>Guía a padres en trámites administrativos.</li>
          <li>Opera las 24 horas a través de WhatsApp Business.</li>
          <li>Gestiona solicitudes y registros en tiempo real.</li>
        </ul>
      </section>
      <section>
        <h2>Tecnología usada</h2>
        <ul>
          <li>WhatsApp Business API como canal principal.</li>
          <li>Evolution API y Make para la automatización de flujos.</li>
          <li>Bases de datos relacionales para la gestión de información.</li>
        </ul>
      </section>
      <section>
        <h2>Equipo de Desarrollo</h2>
        <ul>
          <li>David Quintana – Programador y líder de innovación.</li>
          <li>Ashly Rueda – Diseñadora UX/UI.</li>
          <li>Paula Cadena – Analista funcional.</li>
        </ul>
      </section>
      <section>
        <h2>Valores del Proyecto</h2>
        <ul>
          <li>Innovación con propósito.</li>
          <li>Servicio con fe.</li>
          <li>Colaboración.</li>
          <li>Excelencia y mejora continua.</li>
        </ul>
      </section>
      <section>
        <h2>Relación con los ODS</h2>
        <p>El proyecto se alinea con el ODS 9 (Industria, Innovación e Infraestructura) al fomentar la cultura digital y el uso de tecnologías emergentes dentro del entorno escolar.</p>
      </section>
      <section>
        <h2>Impacto esperado</h2>
        <ul>
          <li>Reducir los tiempos de espera en secretarías escolares.</li>
          <li>Mejorar la atención a padres y estudiantes con un sistema disponible 24/7.</li>
          <li>Promover en los estudiantes el desarrollo de habilidades digitales y tecnológicas.</li>
          <li>Convertir a SALI en un referente de innovación educativa en Iberoamérica.</li>
        </ul>
      </section>
      <section>
        <h2>Conclusión</h2>
        <p>SALI es una solución tecnológica integral que moderniza la administración escolar, promueve la innovación y fortalece la relación entre colegio, estudiantes y padres de familia.</p>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 0;
}

.top-bar {
  background: #f5f5f5;
  padding: 1rem;
}

.nav-links {
  display: flex;
  justify-content: flex-end;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav-links li + li {
  margin-left: 1rem;
}

.nav-link {
  text-decoration: none;
  color: #42b983;
}

.content {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  text-align: left;
}
</style>
