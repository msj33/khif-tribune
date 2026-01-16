---
layout: default
title: "Forside"
---

<div class="homepage-container">
  <h1>KHIF Tribunen</h1>

  <p>Kolt-Hasselager IF Fodbold arbejder aktivt for at bygge en tilskuer-tribune, som skal styrke fællesskabet samt gøre rammerne for vores klub endnu bedre.</p>

  {% include progressbar.html belob=site.data.donationer.belob total=605000 %}

  <p>Læs mere om projektet og se hvem der støtter os via menuen</p>

  <!-- Kursiv note før billedet -->
  <p style="font-size: 0.9em; font-style: italic; color: #ddd;">
    *Billedet er en idéskitse og viser ikke det færdige resultat*
  </p>

  <img src="{{ '/assets/khif_tribune.png' | relative_url }}" alt="Ny tribune" class="tribune-image">

  <p class="last-updated">
    Sidst opdateret: {{ site.data.donationer.sidst_opdateret }}
  </p>
</div>

