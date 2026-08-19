<template>
  <section>
    <h1>Personenkarten</h1>

    <article>
      <h2>Dmytro Yermakov</h2>
      <p><strong>Rolle:</strong> Frontend Developer</p>

      <h3>Stärken</h3>
      <ul>
        <li>Logisches Denken</li>
        <li>Vue.js / Komponentenentwicklung</li>
        <li>JS / Frontend-Logik</li>
      </ul>

      <h3>Schwächen</h3>
      <ul>
        <li>SQL / Datenbanken</li>
      </ul>
    </article>

    <article>
      <h2>Fabio Erculiani</h2>
      <p><strong>Rolle:</strong> Database Manager</p>

      <h3>Stärken</h3>
      <ul>
        <li>SQL/Datenbanken managen</li>
        <li>JS/Webseitenlogik</li>
        <li>HTML/Struktur</li>
      </ul>

      <h3>Schwächen</h3>
      <ul>
        <li>CSS/Gestaltung</li>
      </ul>
    </article>

    <article>
      <h2>Liam</h2>
      <p><strong>Rolle:</strong> Backend Developer</p>

      <h3>Stärken</h3>
      <ul>
        <li>Java und Backend-Logik</li>
        <li>APIs entwickeln</li>
        <li>Fehler finden und lösen</li>
      </ul>

      <h3>Schwächen</h3>
      <ul>
        <li>Noch nicht viel Erfahrung mit grösseren Backend-Systemen</li>
        <li>Dokumentation könnte konsequenter sein</li>
      </ul>
    </article>

    <article>
      <h2>Boris Tomovski</h2>
      <p><strong>Rolle:</strong> Projektleiter/Frontend</p>

      <h3>Stärken</h3>
      <ul>
        <li>Schnelles Debugging & Problemlösung</li>
        <li>Frontend Design</li>
        <li>Projektleitung</li>
      </ul>

      <h3>Schwächen</h3>
      <ul>
        <li>Over Engineering</li>
        <li>Wenig Erfahrung mit Backend</li>
      </ul>
    </article>
  </section>
</template>

<style scoped>
section {
  width: min(100%, 1000px);
  margin: 0 auto;
  padding: 40px 20px;
}

h1 {
  margin-bottom: 24px;
  text-align: center;
}

article {
  margin-bottom: 20px;
  padding: 24px;
  border: 1px solid #d6dbe1;
  border-radius: 10px;
  background-color: #ffffff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.06);
}

h2 {
  margin-bottom: 12px;
}

p {
  margin-bottom: 16px;
}

h3 {
  margin: 16px 0 8px;
}

ul {
  padding-left: 24px;
  min-height: 72px;
}

li {
  min-height: 24px;
}
</style>