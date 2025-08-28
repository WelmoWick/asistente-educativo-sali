<template>
  <!-- Accesibilidad: link para saltar al contenido -->
  <a class="skip-link" href="#hero">Saltar al contenido</a>

  <!-- ====== HEADER / NAV ====== -->
  <header class="site-header" role="banner">
    <div class="container header-inner">
      <div class="brand">
        <span class="brand-logo" aria-hidden="true">🤖</span>
        <span class="brand-name">SALI — Asistente Educativo</span>
      </div>

      <!-- Encapsulamos nav + accesos directos a la derecha -->
      <div class="header-right">
        <nav class="main-nav" role="navigation" aria-label="Navegación principal">
          <ul>
            <li><a href="#beneficios">Beneficios</a></li>
            <li><a href="#funcionalidades">Funcionalidades</a></li>
            <li><a href="#como-funciona">Cómo funciona</a></li>
            <li><a href="#tecnologia">Tecnología</a></li>
            <li><a href="#faq">FAQ</a></li>
            <li><a class="btn btn-primary btn-small" href="#contacto">Solicitar demo</a></li>
          </ul>
        </nav>

        <!-- ACCESOS DIRECTOS -->
        <div class="quick-links" aria-label="Accesos directos">
          <!-- Google Drive -->
          <a
            class="icon-btn"
            :href="driveUrl"
            target="_blank"
            rel="noopener"
            aria-label="Abrir carpeta de Google Drive"
            title="Google Drive"
          >
            <svg class="icon-svg icon-drive" viewBox="0 0 24 24" aria-hidden="true">
              <path d="M3.5 2l5.5 9.5L3.5 21h5.5L15 11.5 9.5 2H3.5zm6 0L15 11.5l5.5-9.5H9.5zm5.5 9.5L9.5 21H21l-6-9.5z" />
            </svg>
          </a>

          <!-- WhatsApp -->
          <a
            class="icon-btn"
            :href="whatsUrl"
            target="_blank"
            rel="noopener"
            aria-label="Chatear por WhatsApp"
            title="WhatsApp"
          >
            <svg class="icon-svg icon-whatsapp" viewBox="0 0 24 24" aria-hidden="true">
              <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.472-.148-.672.15-.198.297-.767.966-.94 1.164-.173.198-.347.223-.644.074-.297-.149-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.52.149-.173.198-.297.298-.495.099-.198.05-.372-.025-.521-.075-.149-.672-1.612-.921-2.207-.242-.58-.487-.501-.672-.51l-.572-.01c-.198 0-.52.074-.792.372-.273.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.095 3.2 5.076 4.487.709.306 1.262.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.408h-.003a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.22c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.896 6.98c-.003 5.45-4.437 9.884-9.889 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L0 24l6.305-1.654a11.87 11.87 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.82 11.82 0 00-3.492-8.413"/>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </header>

  <main id="contenido" tabindex="-1">
    <!-- ====== HERO ====== -->
    <section id="hero" class="section hero" aria-labelledby="hero-title">
      <div class="container hero-inner">
        <div class="hero-copy">
          <p class="eyebrow">Asistente educativo por WhatsApp</p>
          <h1 id="hero-title">
            Reduce la carga administrativa del colegio con respuestas inmediatas 24/7
          </h1>
          <p class="subtitle">
            SALI atiende preguntas frecuentes de padres y estudiantes — horarios, matrículas, reuniones,
            precios de uniformes y reglamentos — sin filas ni llamadas.
          </p>
          <ul class="hero-bullets" role="list">
            <li>Hasta 80% menos carga administrativa en FAQs, matrículas y horarios</li>
            <li>Disponibilidad 24/7 para toda la comunidad educativa</li>
            <li>Diseñado para educación; información oficial y consistente</li>
          </ul>
          <div class="cta-group">
            <a class="btn btn-primary" :href="demoUrl" rel="noopener">Probar SALI ahora</a>
            <a class="btn btn-secondary" href="#contacto">Solicitar demo</a>
          </div>
        </div>
        <figure class="hero-media" aria-label="Vista de conversación con SALI">
          <div class="mockup-chat">
            <div class="bubble bubble-in">Hola 👋 ¿Cuáles son los horarios de atención?</div>
            <div class="bubble bubble-out">
              ¡Hola! Nuestro horario de atención es de 7:00 a.m. a 12:00 p.m. y de 2:00 p.m. a 5:00 p.m. 🕒
            </div>
            <div class="bubble bubble-in">¿Cuándo son las matrículas?</div>
            <div class="bubble bubble-out">
              Las matrículas están abiertas del 1 al 15 de septiembre. Aquí los requisitos 👉 PDF
            </div>
          </div>
        </figure>
      </div>
    </section>

    <!-- ====== BENEFICIOS ====== -->
    <section id="beneficios" class="section" aria-labelledby="beneficios-title">
      <div class="container">
        <h2 id="beneficios-title">Beneficios para tu institución</h2>
        <div class="grid cards">
          <article v-for="(b, i) in beneficios" :key="i" class="card">
            <div class="icon" aria-hidden="true">{{ b.icon }}</div>
            <h3 class="card-title">{{ b.title }}</h3>
            <p class="card-text">{{ b.description }}</p>
          </article>
        </div>
      </div>
    </section>

    <!-- ====== FUNCIONALIDADES ====== -->
    <section id="funcionalidades" class="section alt" aria-labelledby="funcionalidades-title">
      <div class="container">
        <h2 id="funcionalidades-title">¿Qué resuelve SALI?</h2>
        <ul class="feature-list" role="list">
          <li v-for="(f, i) in funcionalidades" :key="i">
            <span class="feature-icon" aria-hidden="true">{{ f.icon }}</span>
            <span class="feature-text">{{ f.text }}</span>
          </li>
        </ul>
      </div>
    </section>

    <!-- ====== CÓMO FUNCIONA ====== -->
    <section id="como-funciona" class="section" aria-labelledby="como-title">
      <div class="container">
        <h2 id="como-title">Cómo funciona</h2>
        <ol class="steps" role="list">
          <li v-for="(s, i) in pasos" :key="i">
            <div class="step-num">{{ i + 1 }}</div>
            <div class="step-body">
              <p class="step-label">{{ s.label }}</p>
              <p class="step-desc">{{ s.description }}</p>
            </div>
          </li>
        </ol>
      </div>
    </section>

    <!-- ====== TECNOLOGÍA ====== -->
    <section id="tecnologia" class="section alt" aria-labelledby="tech-title">
      <div class="container">
        <h2 id="tech-title">Tecnología confiable</h2>
        <div class="grid tech">
          <div v-for="(t, i) in stack" :key="i" class="tech-item">
            <h3 class="tech-name">{{ t.name }}</h3>
            <p class="tech-detail">{{ t.detail }}</p>
          </div>
        </div>
      </div>
    </section>

    <!-- ====== DIFERENCIADORES ====== -->
    <section id="diferenciadores" class="section" aria-labelledby="diff-title">
      <div class="container">
        <h2 id="diff-title">Lo que nos hace diferentes</h2>
        <div class="grid cards">
          <article v-for="(d, i) in diferenciadores" :key="i" class="card">
            <h3 class="card-title">{{ d.title }}</h3>
            <p class="card-text">{{ d.description }}</p>
          </article>
        </div>
      </div>
    </section>

    <!-- ====== ODS / PROPÓSITO ====== -->
    <section id="impacto-ods" class="section banner" aria-labelledby="ods-title">
      <div class="container banner-inner">
        <div>
          <h2 id="ods-title">Innovación con propósito</h2>
          <p>
            Alineado con el <strong>ODS 9</strong> (Industria, Innovación e Infraestructura): fomenta cultura digital y
            moderniza procesos escolares.
          </p>
        </div>
      </div>
    </section>

    <!-- ====== CTA MEDIO ====== -->
    <section id="cta-medio" class="section cta" aria-labelledby="cta-title">
      <div class="container cta-inner">
        <div>
          <h2 id="cta-title">¿Listos para liberar a la secretaría de preguntas repetidas?</h2>
          <p>Implementa SALI y mejora la atención a padres y estudiantes desde esta semana.</p>
        </div>
        <div class="cta-actions">
          <a class="btn btn-primary" :href="demoUrl">Probar SALI</a>
          <a class="btn btn-secondary" href="#contacto">Solicitar demo</a>
        </div>
      </div>
    </section>

    <!-- ====== FAQ ====== -->
    <section id="faq" class="section alt" aria-labelledby="faq-title">
      <div class="container">
        <h2 id="faq-title">Preguntas frecuentes</h2>
        <div class="accordion" role="list">
          <details v-for="(item, i) in faq" :key="i" class="accordion-item" @toggle="onToggle(i, $event)">
            <summary class="accordion-summary">
              <span class="q">{{ item.q }}</span>
              <span class="marker" aria-hidden="true">+</span>
            </summary>
            <div class="accordion-panel">
              <p class="a">{{ item.a }}</p>
            </div>
          </details>
        </div>
      </div>
    </section>

    <!-- ====== CONTACTO ====== -->
    <section id="contacto" class="section" aria-labelledby="contacto-title">
      <div class="container">
        <h2 id="contacto-title">Solicitar una demo</h2>
        <p class="contact-subtitle">Déjanos tus datos y te contactamos para activar SALI en tu institución.</p>
        <form class="form" @submit.prevent="handleSubmit" novalidate>
          <div class="grid form-grid">
            <label class="field">
              <span>Nombre *</span>
              <input v-model.trim="form.nombre" type="text" name="nombre" required autocomplete="name" />
            </label>
            <label class="field">
              <span>Correo *</span>
              <input v-model.trim="form.email" type="email" name="email" required autocomplete="email" />
            </label>
            <label class="field">
              <span>Teléfono</span>
              <input v-model.trim="form.telefono" type="tel" name="telefono" autocomplete="tel" />
            </label>
            <label class="field">
              <span>Institución *</span>
              <input v-model.trim="form.colegio" type="text" name="colegio" required />
            </label>
          </div>
          <label class="field">
            <span>Mensaje</span>
            <textarea v-model.trim="form.mensaje" name="mensaje" rows="4" placeholder="Cuéntanos brevemente tus necesidades"></textarea>
          </label>

          <div class="form-actions">
            <button class="btn btn-primary" type="submit">Enviar</button>
            <p v-if="submitted" class="form-feedback" role="status">
              ¡Gracias! Hemos recibido tu solicitud. Nos pondremos en contacto pronto.
            </p>
          </div>
        </form>
      </div>
    </section>
  </main>

  <!-- ====== FOOTER ====== -->
  <footer class="site-footer" role="contentinfo">
    <div class="container footer-inner">
      <p>© 2025 SALI</p>
      <nav aria-label="Enlaces de pie">
        <ul class="footer-links">
          <li><a :href="demoUrl">Probar SALI</a></li>
          <li><a href="#contacto">Solicitar demo</a></li>
          <li><a href="#faq">FAQ</a></li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<script setup>
/* global defineOptions */
defineOptions({ name: 'SALI_Landing' });

import { reactive, ref } from 'vue';

const demoUrl = 'https://asistente-educativo-sali.vercel.app';
const driveUrl = 'https://drive.google.com/drive/folders/14jt4USrqAt03RYeWelzmzx1ZJO1k-2Xi?usp=sharing';
const whatsUrl = 'https://wa.me/573142802136';

const beneficios = [
  { icon: '⚡', title: 'Atención sin esperas', description: 'Consultas respondidas al instante en WhatsApp para reducir filas y llamadas.' },
  { icon: '✅', title: 'Información confiable', description: 'Respuestas oficiales y estandarizadas para toda la comunidad.' },
  { icon: '📈', title: 'Eficiencia operativa', description: 'Secretaría con más tiempo para tareas de mayor valor.' },
  { icon: '🌐', title: 'Disponibilidad 24/7', description: 'SALI nunca se detiene: soporte continuo todo el año.' }
];

const funcionalidades = [
  { icon: '💬', text: 'Preguntas frecuentes: horarios, matrículas, reuniones, precios de uniformes y reglamentos.' },
  { icon: '🗓️', text: 'Fechas y recordatorios académicos siempre al día.' },
  { icon: '🧭', text: 'Guías paso a paso para trámites y solicitudes.' },
  { icon: '🗄️', text: 'Gestión de solicitudes y registros en tiempo real con base de datos relacional.' }
];

const pasos = [
  { label: 'WhatsApp Business', description: 'Canal principal de comunicación directo con padres y estudiantes.' },
  { label: 'Automatización con Make + Evolution API', description: 'Orquestación de flujos y menús interactivos para respuestas rápidas.' },
  { label: 'Base de datos institucional', description: 'Usuarios, FAQs, solicitudes y datos oficiales para respuestas consistentes.' }
];

const stack = [
  { name: 'WhatsApp Business API', detail: 'Canal oficial y masivo para atención.' },
  { name: 'Make (Integromat)', detail: 'Automatización de procesos y webhooks.' },
  { name: 'Evolution API', detail: 'Conectores robustos para continuidad del servicio.' },
  { name: 'Bases de datos relacionales', detail: 'FAQs, usuarios, solicitudes e información institucional.' }
];

const diferenciadores = [
  { title: 'Hecho para educación', description: 'Diseñado según valores y necesidades de la comunidad educativa.' },
  { title: 'Continuidad operativa', description: 'Arquitectura con Evolution API + Make para alta disponibilidad.' },
  { title: 'Escalable y adaptable', description: 'Listo para crecer y ajustarse a tu institución.' }
];

const faq = [
  { q: '¿Funciona por WhatsApp?', a: 'Sí. SALI opera en WhatsApp Business como canal principal para padres y estudiantes.' },
  { q: '¿Está disponible 24/7?', a: 'Sí. El asistente responde consultas a cualquier hora, todos los días.' },
  { q: '¿Qué tipo de preguntas responde?', a: 'Horarios, eventos, matrículas, reuniones, precios de uniformes, reglamentos y más.' },
  { q: '¿Con qué tecnología está construido?', a: 'WhatsApp Business API, Make y Evolution API; respaldo en bases de datos relacionales.' },
  { q: '¿Cómo garantiza respuestas consistentes?', a: 'Mediante una base de preguntas y respuestas oficiales (FAQs) y datos institucionales actualizados.' }
];

let openIndex = -1;
function onToggle(i, evt) { openIndex = evt.target.open ? i : (openIndex === i ? -1 : openIndex); }

const form = reactive({ nombre: '', email: '', telefono: '', colegio: '', mensaje: '' });
const submitted = ref(false);

function handleSubmit() {
  if (!form.nombre || !form.email || !form.colegio) {
    alert('Por favor completa los campos obligatorios (Nombre, Correo, Institución).');
    return;
  }
  const params = new URLSearchParams({
    subject: 'Solicitud de demo SALI',
    body: `Nombre: ${form.nombre}\nCorreo: ${form.email}\nTeléfono: ${form.telefono}\nInstitución: ${form.colegio}\nMensaje: ${form.mensaje}`
  });
  window.location.href = `mailto:saliasistenteeducativo@gmail.com?${params.toString()}`;
  submitted.value = true;
  form.nombre = form.email = form.telefono = form.colegio = form.mensaje = '';
  setTimeout(() => (submitted.value = false), 6000);
}
</script>

<style scoped>
  :root {
    --bg: #111a2e;
    --bg-alt: #18253d;
    --card: #1f2e4a;
    --text: #e6eefc;
    --muted: #aab8d0;
    --primary: #1e3a8a;
    --primary-2: #0ea5e9;
    --ring: rgba(14, 165, 233, 0.35);
  }

* { box-sizing: border-box; }
html, body, :host { background: var(--bg); color: var(--text); font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji", "Segoe UI Emoji"; }
a { color: var(--primary-2); text-decoration: none; }
a:hover { text-decoration: underline; }

.container { width: min(1120px, 92vw); margin: 0 auto; }
.section { padding: 64px 0; }
.section.alt { background: var(--bg-alt); }

h1, h2, h3 { line-height: 1.15; margin: 0 0 12px; }
h1 { font-size: clamp(28px, 3.4vw, 40px); }
h2 { font-size: clamp(22px, 2.6vw, 30px); }
h3 { font-size: clamp(18px, 2.2vw, 24px); }

.eyebrow { text-transform: uppercase; letter-spacing: .12em; font-size: 12px; color: var(--muted); }
.subtitle { color: var(--muted); margin: 8px 0 16px; }

/* Header */
  .site-header { position: sticky; top: 0; z-index: 20; background: rgba(32, 45, 70, 0.7); backdrop-filter: blur(8px); border-bottom: 1px solid rgba(255,255,255,.06); }
.header-inner { display: flex; align-items: center; justify-content: space-between; padding: 12px 0; }
.brand { display: flex; align-items: center; gap: 8px; font-weight: 700; }
.brand-logo { font-size: 20px; }
.brand-name { font-size: 16px; }

/* Header right (nav + quick links) */
.header-right { display: flex; align-items: center; gap: 12px; }
.main-nav ul { display: flex; gap: 16px; list-style: none; margin: 0; padding: 0; }
.main-nav a { padding: 8px 10px; border-radius: 8px; }
.main-nav a:hover { background: rgba(255,255,255,.05); text-decoration: none; }

/* Quick links top-right */
.quick-links { display: flex; gap: 8px; }
.icon-btn {
  width: 38px; height: 38px; display: grid; place-items: center;
  border-radius: 10px; background: var(--card); border: 1px solid rgba(255,255,255,.08);
  box-shadow: 0 4px 16px rgba(0,0,0,.25);
}
  .icon-btn:hover { background: #1d3c6b; }
.icon-svg { width: 20px; height: 20px; }
.icon-whatsapp { fill: #25D366; }

/* Buttons */
.btn {
  display: inline-flex; align-items: center; justify-content: center;
  padding: 12px 18px; border-radius: 12px; font-weight: 700;
  border: 1px solid transparent; text-decoration: none;
  transition: transform .04s ease, box-shadow .2s ease, background .2s ease, border-color .2s ease;
  box-shadow: 0 6px 20px rgba(14, 165, 233, .12);
}
.btn:hover { transform: translateY(-1px); text-decoration: none; }
.btn:focus-visible { outline: 3px solid var(--ring); outline-offset: 2px; }
.btn-small { padding: 8px 12px; font-size: 14px; }
.btn-primary { background: linear-gradient(135deg, var(--primary) 0%, var(--primary-2) 100%); color: #fff; }
.btn-primary:hover { filter: brightness(1.06); }
.btn-secondary { background: transparent; color: var(--primary-2); border-color: var(--primary-2); }
.btn-secondary:hover { background: rgba(14,165,233,.1); }

/* Hero */
.hero { padding: 80px 0 40px; }
.hero-inner { display: grid; gap: 28px; align-items: center; grid-template-columns: 1.1fr .9fr; }
.hero-bullets { margin: 8px 0 20px; padding-left: 18px; color: var(--text); }
.cta-group { display: flex; gap: 12px; flex-wrap: wrap; }
.hero-media { display: flex; justify-content: center; }
    .mockup-chat {
      width: 100%; max-width: 420px; background: #223a60; border: 1px solid rgba(255,255,255,.06);
      border-radius: 16px; padding: 16px; box-shadow: 0 10px 30px rgba(0,0,0,.25);
    }
    .bubble { padding: 10px 12px; border-radius: 12px; margin: 8px 0; line-height: 1.35; }
    .bubble-in { background: #264a80; align-self: flex-start; }
    .bubble-out { background: #25537f; border-left: 3px solid var(--primary-2); }

/* Cards / Grid */
.grid { display: grid; gap: 16px; }
.cards { grid-template-columns: repeat(auto-fit, minmax(230px, 1fr)); }
.card { background: var(--card); border: 1px solid rgba(255,255,255,.06); border-radius: 16px; padding: 16px; }
.card-title { margin-bottom: 6px; }
.card-text { color: var(--muted); }
.icon { font-size: 22px; }

/* Feature list */
.feature-list { display: grid; gap: 12px; }
.feature-list li { display: grid; grid-template-columns: 28px 1fr; gap: 10px; align-items: start; background: var(--card); border: 1px solid rgba(255,255,255,.06); border-radius: 14px; padding: 12px; }
.feature-icon { font-size: 18px; }

/* Steps */
.steps { display: grid; gap: 12px; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); counter-reset: step; list-style: none; padding: 0; }
.step-num {
  width: 36px; height: 36px; border-radius: 11px; display: grid; place-items: center;
  background: linear-gradient(135deg, var(--primary), var(--primary-2)); font-weight: 800;
}
.step-body { margin-top: 8px; }
.step-label { font-weight: 700; margin: 6px 0 4px; }
.step-desc { color: var(--muted); }

/* Tech stack */
.tech { grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); }
.tech-item { background: var(--card); padding: 16px; border-radius: 16px; border: 1px solid rgba(255,255,255,.06); }
.tech-name { margin: 0 0 4px; }

/* Banner / ODS */
.banner { background: linear-gradient(135deg, rgba(30,58,138,.35), rgba(14,165,233,.2)); }
.banner-inner { display: grid; gap: 10px; }

/* CTA middle */
.cta { background: var(--bg-alt); }
.cta-inner { display: grid; gap: 16px; align-items: center; grid-template-columns: 1fr auto; }
.cta-actions { display: flex; gap: 12px; }

/* Accordion (FAQ) */
.accordion-item { background: var(--card); border: 1px solid rgba(255,255,255,.06); border-radius: 14px; margin-bottom: 10px; overflow: hidden; }
.accordion-summary { list-style: none; cursor: pointer; padding: 14px 16px; display: flex; align-items: center; justify-content: space-between; }
.accordion-summary::-webkit-details-marker { display: none; }
.accordion-panel { padding: 0 16px 14px; color: var(--muted); }
.marker { font-weight: 700; }
details[open] .marker { transform: rotate(45deg); }

/* Form */
.form { margin-top: 10px; }
.form-grid { grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); }
.field { display: grid; gap: 6px; margin-bottom: 12px; }
  .field input, .field textarea {
    width: 100%; padding: 12px 14px; border-radius: 12px; border: 1px solid rgba(255,255,255,.1);
    background: #223a60; color: var(--text);
  }
.field input:focus, .field textarea:focus { outline: 3px solid var(--ring); border-color: var(--primary-2); }
.form-actions { display: flex; gap: 12px; align-items: center; flex-wrap: wrap; }
.form-feedback { color: #b7ffb7; }

/* Footer */
.site-footer { border-top: 1px solid rgba(255,255,255,.06); padding: 28px 0; margin-top: 40px; }
.footer-inner { display: flex; align-items: center; justify-content: space-between; gap: 12px; flex-wrap: wrap; }
.footer-links { display: flex; gap: 12px; list-style: none; margin: 0; padding: 0; }

/* Helpers */
.skip-link { position: absolute; left: 8px; top: -40px; background: #fff; color: #111; padding: 8px 10px; border-radius: 8px; }
.skip-link:focus { top: 8px; }

@media (max-width: 900px) {
  .hero-inner { grid-template-columns: 1fr; }
  .cta-inner { grid-template-columns: 1fr; }
  .header-right { gap: 8px; }
}

@media (max-width: 600px) {
  .header-inner { flex-wrap: wrap; }
  .header-right { width: 100%; justify-content: space-between; }
  .main-nav ul { flex-wrap: wrap; justify-content: center; }
}
</style>
