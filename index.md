---
layout: default
title: "Forside"
---

<div class="homepage-container">
  <h1>Støt KHIF Tribunen</h1>

  <p>Kolt-Hasselager IF Fodbold planlægger at bygge en tribune, som skal styrke fællesskabet samt gøre rammerne for vores klub endnu bedre.</p>

  {% include progressbar.html belob=site.data.donationer.belob total=500000 %}

  <p>Se de enkelte donationer/fondsmidler, Vær med til at støtte og læs meget mere om projektet via menuen</p>

    <!-- Kursiv note før billedet -->
  <p style="font-size: 0.9em; font-style: italic; color: #ddd;">
    *Billedet er en idéskitse og viser ikke det færdige resultat*
  </p>

  <img src="{{ '/assets/khif_tribune.png' | relative_url }}" alt="Ny tribune" class="tribune-image">

  <p class="last-updated">
    Sidst opdateret: {{ site.data.donationer.sidst_opdateret }}
  </p>
</div>

