---
layout: page
permalink: /repositories/
title: repositories
description: Library of my open-sourced contribution
nav: true
nav_order: 4
---

<link rel="preconnect" href="https://cdn.jsdelivr.net">
<link rel="preconnect" href="https://api.observablehq.com">

<style>
.custom-github-pins {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: left;
  gap: 1.5rem;
  margin-top: 1.5rem;
}

.github-pin-card {
  width: 45%;
  display: flex;
  flex-direction: column;
}

.github-pin-card h2 {
  margin-bottom: 0.75rem;
}

.github-pin-image {
  height: 180px;
  width: 100%;
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  /* transition: transform 0.2s ease, box-shadow 0.2s ease; */
}

/* .github-pin-image:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.12);
} */

.github-pin-image img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.github-pin-image img:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.12);
}

@media (max-width: 767px) {
  .custom-github-pins {
    flex-direction: column;
  }

  .github-pin-card {
    width: 100%;
  }
}

.notion-embed {
  width: 50%;
  height: 400px;
  overflow: hidden;
}

@media (max-width: 767px) {
  .notion-embed {
    width: 100%;
  }
}
</style>

## Github

<div class="custom-github-pins">

  <div class="github-pin-card">
    <h3>Profile</h3>

    <a href="https://github.com/SRituparna">
      <div class="github-pin-image">
        <img
          loading="lazy"
          src="https://github-stats-extended.vercel.app/api/top-langs?username=SRituparna&layout=compact&langs_count=4&hide_values=true&theme=default&disable_animations=True&card_width=400&custom_title=github.com/SRituparn"
          alt="Rituparna">
      </div>
    </a>
  </div>
</div>

---

<div class="custom-github-pins">
  <div class="github-pin-card">
    <h3>Github Repo</h3>

    <a href="https://github.com/postDoc-potential/postdoc-potential.github.io">
      <div class="github-pin-image">
        <img
          loading="lazy"
          src="https://github-stats-extended.vercel.app/api/pin?username=SRituparna&repo=postDoc-potential%2Fpostdoc-potential.github.io&description_lines_count=3&browser_rendering=true&card_width=450"
          alt="GitHub repository">
      </div>
    </a>
  </div>

</div>

---

## Google App Script

<div class="custom-github-pins">
  <div class="github-pin-card">
  
    <a href="https://github.com/SRituparna/surveyJS-spreadsheet-connector-api">
      <div class="github-pin-image">
        <img
          loading="lazy" alt="SurveyJS Spreadsheet Connector repository card" 
          src="https://github-stats-extended.vercel.app/api/pin?username=SRituparna&repo=SRituparna%2FsurveyJS-spreadsheet-connector-api&show_icons=true&card_width=400">
      </div>
    </a>
  </div>
</div>

---

## Observable Notebook

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@observablehq/inspector@5/dist/inspector.css">

<div style="width:50%; height:400px; overflow:hidden;">  
  <h3><a href="https://observablehq.com/d/1c11066aa24ae815@151">Packed Circle Chart</a></h3>
  <p>By <a href="https://old.observablehq.com/@rituparna-sarkar?tab=recents">rituparna-sarkar</a></p>
  <div id="observablehq-embed-d7a99c2b"></div>
</div>

<script type="module">
  document.addEventListener("DOMContentLoaded", () => {
    const target = document.querySelector("#observablehq-embed-d7a99c2b");
    if (!target) return;

    const NOTEBOOK_URL = "https://api.observablehq.com/d/1c11066aa24ae815@151.js?v=4&api_key=08b4923e63ed3a3ca66baed640fbfac61ce43102";
    const RUNTIME_URL = "https://cdn.jsdelivr.net/npm/@observablehq/runtime@5/dist/runtime.js";

    function loadChart() {
      Promise.all([
        import(RUNTIME_URL),
        import(NOTEBOOK_URL)
      ])
        .then(([{ Runtime, Inspector }, module]) => {
          new Runtime().module(module.default, (name) => {
            if (name === "embed") return new Inspector(target);
          });
        })
        .catch((err) => {
          console.error("Observable embed failed to load:", err);
          target.innerHTML =
            "<p style='color:#888;font-size:0.9em;'>Chart unavailable — " +
            "<a href='https://observablehq.com/d/1c11066aa24ae815@151'>view on Observable</a>.</p>";
        });
    }

    if ("IntersectionObserver" in window) {
      const observer = new IntersectionObserver(
        (entries) => {
          if (!entries[0].isIntersecting) return;
          observer.disconnect();
          loadChart();
        },
        { rootMargin: "200px" }
      );
      observer.observe(target);
    } else {
      loadChart();
    }
  });
</script>

---

## Notion Template

<iframe
  class="notion-embed"
  loading="lazy"
  title="Movie Database: Notion Template Preview"
  src="https://personalaccountsofameteorologist.notion.site/ebd/64c563ec53a544699d572c9f04bc8dab?v=c4410bb809164632b918eeb9da594358"
  frameborder="0"
  allowfullscreen>
</iframe>