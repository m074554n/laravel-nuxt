<template>
  <main class="page-shell">
    <NuxtRouteAnnouncer />

    <section class="intro">
      <p class="eyebrow">Laravel + Nuxt Demo</p>
      <h1>Deploying Laravel and Nuxt with Forge</h1>
      <p class="summary">
        A compact example for showing how a Laravel backend and Nuxt frontend
        can be prepared, deployed, and supported through Laravel Forge.
      </p>
    </section>

    <section class="content-grid" aria-label="Deployment overview">
      <article>
        <span>01</span>
        <h2>Laravel Backend</h2>
        <p>
          Configure the Laravel application, review environment variables, and
          confirm the backend is ready for the production server.
        </p>
      </article>

      <article>
        <span>02</span>
        <h2>Nuxt Frontend</h2>
        <p>
          Build the Nuxt application, define the runtime settings, and make sure
          the frontend can communicate with the Laravel API.
        </p>
      </article>

      <article>
        <span>03</span>
        <h2>Forge Deployment</h2>
        <p>
          Use Forge to connect the repository, set the deployment commands, and
          keep both Laravel and Nuxt running predictably.
        </p>
      </article>
    </section>
  </main>
</template>

<style>
:root {
  color: #111827;
  background: #fff7f5;
  font-family:
    Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
    sans-serif;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
}

.page-shell {
  min-height: 100vh;
  padding: 72px 24px;
  background:
    linear-gradient(180deg, rgba(255, 45, 32, 0.1), transparent 42%),
    #fff7f5;
}

.intro,
.content-grid {
  width: min(960px, 100%);
  margin: 0 auto;
}

.intro {
  padding-bottom: 56px;
  border-bottom: 1px solid rgba(255, 45, 32, 0.22);
}

.eyebrow {
  margin: 0 0 18px;
  color: #ff2d20;
  font-size: 0.82rem;
  font-weight: 800;
  letter-spacing: 0.12em;
  text-transform: uppercase;
}

h1,
h2,
p {
  margin-top: 0;
}

h1 {
  max-width: 780px;
  margin-bottom: 22px;
  color: #1f2937;
  font-size: clamp(2.75rem, 7vw, 5.75rem);
  line-height: 0.95;
  letter-spacing: 0;
}

.summary {
  max-width: 620px;
  margin-bottom: 0;
  color: #4b5563;
  font-size: 1.22rem;
  line-height: 1.7;
}

.content-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 20px;
  padding-top: 32px;
}

article {
  padding: 28px;
  border: 1px solid rgba(255, 45, 32, 0.18);
  border-radius: 8px;
  background: rgba(255, 255, 255, 0.78);
}

article span {
  display: block;
  margin-bottom: 24px;
  color: #ff2d20;
  font-size: 0.86rem;
  font-weight: 800;
}

h2 {
  margin-bottom: 12px;
  color: #111827;
  font-size: 1.12rem;
}

article p {
  margin-bottom: 0;
  color: #5b6472;
  line-height: 1.65;
}

@media (max-width: 760px) {
  .page-shell {
    padding: 48px 18px;
  }

  .intro {
    padding-bottom: 40px;
  }

  .content-grid {
    grid-template-columns: 1fr;
  }

  article {
    padding: 24px;
  }
}
</style>
