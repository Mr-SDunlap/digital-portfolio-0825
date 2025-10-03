<script setup></script>

<template>
  <main>
    <header class="site">
      <nav class="nav">
        <a class="logo" href="/">SD</a>
        <div class="links">
          <a href="#work">Work</a>
          <a href="#templates">Templates</a>
          <a href="#about">About</a>
          <a href="#contact" class="button button--primary">Contact</a>
        </div>
      </nav>

      <section class="hero">
        <h1>Design that’s calm, clear, and fast to ship.</h1>
        <p>
          I build simple, modern sites and templates that help creatives look
          professional and get paid.
        </p>
        <div class="cta">
          <a href="/templates" class="button button--primary">Shop Templates</a>
          <a href="#work" class="button button--ghost">See Work</a>
        </div>
      </section>
    </header>

    <section id="work" class="section">
      <h2>Selected work</h2>
      <p class="sub">
        A few quick snapshots. Email me if you want the nuts and bolts.
      </p>
      <div class="grid">
        <article class="card">
          <h3>NaaS Quiz</h3>
          <p>Interactive lead-gen with clean analytics.</p>
        </article>
        <article class="card">
          <h3>Portfolio v3</h3>
          <p>Liquid-glass aesthetic, fast and accessible.</p>
        </article>
        <article class="card">
          <h3>Photo Grid</h3>
          <p>Lazy-loaded gallery with sharp metadata.</p>
        </article>
      </div>
    </section>

    <section id="templates" class="section">
      <h2>Templates that get you unstuck</h2>
      <p class="sub">
        ATS-friendly resumes and clean portfolio layouts. Edit in Figma, ship
        today.
      </p>
      <div class="grid">
        <article class="card">
          <h3>Minimalist Resume (Figma)</h3>
          <p>Plain-text friendly, modern typography.</p>
          <a class="button button--primary" href="https://gumroad.com/YOUR-LINK"
            >View on Gumroad</a
          >
        </article>
        <article class="card">
          <h3>Creative Resume (Figma)</h3>
          <p>Soft pastel accent, readable layout.</p>
          <a class="button button--primary" href="https://gumroad.com/YOUR-LINK"
            >View on Gumroad</a
          >
        </article>
        <article class="card">
          <h3>Portfolio Pack (HTML/Figma)</h3>
          <p>Hero + case grid + about. Ready to ship.</p>
          <a class="button button--primary" href="https://gumroad.com/YOUR-LINK"
            >View on Gumroad</a
          >
        </article>
      </div>
    </section>

    <section id="about" class="section">
      <h2>Hi, I’m Stephen.</h2>
      <p>
        I’m a designer/dev who cares about clarity, speed, and accessible
        polish. I like pastel glassy UI with strong contrast and zero fluff. If
        you’re overwhelmed, my work is the shortcut button.
      </p>
    </section>

    <section id="contact" class="section">
      <h2>Let’s make something simple that works</h2>
      <div class="cta">
        <a class="button button--primary" href="mailto:you@yourdomain.com"
          >Email me</a
        >
        <a class="button button--ghost" href="https://calendly.com/YOUR-LINK"
          >Book 15-min call</a
        >
      </div>
    </section>

    <footer class="footer">
      <p>
        © {{ new Date().getFullYear() }} Stephen Dunlap ·
        <a href="/privacy">Privacy</a>
      </p>
    </footer>
  </main>
</template>

<style>
/* tokens */
:root {
  --sd-diamond: #f0f2f8;
  --ink: #0f172a;
  --coral: #ff6b6b;
  --success: #17b26a;
  --link: #2563eb;
  --muted: #64748b;
}
* {
  box-sizing: border-box;
}
body,
html,
#app {
  margin: 0;
  padding: 0;
  background: var(--sd-diamond);
  color: var(--ink);
  font: 16px/1.5 system-ui, -apple-system, Inter, Segoe UI, Roboto;
}
main {
  max-width: 1100px;
  margin: 0 auto;
  padding: 2rem;
}
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 2rem;
}
.logo {
  font-weight: 800;
  text-decoration: none;
  color: var(--ink);
}
.links a {
  margin-left: 1rem;
  text-decoration: none;
}
.hero {
  padding: 3rem 0;
}
.hero h1 {
  font-size: 2.2rem;
  margin: 0 0 0.5rem;
}
.hero p {
  color: var(--muted);
  max-width: 56ch;
}
.cta {
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
}
.section {
  padding: 3rem 0;
}
.section h2 {
  margin: 0 0 0.25rem;
}
.section .sub {
  color: var(--muted);
  margin: 0 0 1rem;
}
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1rem;
}
.card {
  background: #fff;
  border-radius: 1rem;
  padding: 1rem;
  box-shadow: 0 8px 30px rgba(15, 23, 42, 0.06);
}
.button {
  padding: 0.75rem 1rem;
  border-radius: 0.75rem;
  display: inline-block;
  text-decoration: none;
}
.button--primary {
  background: var(--ink);
  color: #fff;
}
.button--ghost {
  border: 1px solid var(--ink);
  color: var(--ink);
}
.footer {
  padding: 2rem 0;
  color: var(--muted);
}
</style>
