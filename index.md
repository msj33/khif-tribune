---
layout: default
title: "Forside"
---

<div class="homepage-container">
  <h1>KHIF Tribunen</h1>

  <p>Kolt-Hasselager IF Fodbold arbejder aktivt for at bygge en tilskuer-tribune, som skal styrke fællesskabet samt gøre rammerne for vores klub endnu bedre.</p>

  <h2 style="text-align: center; margin-bottom: 10px;">
  Finansieringsbarometer
  </h2>

  <div class="homepage-container">
  {% include progressbar.html
     belob=site.data.donationer.belob
     total=site.data.donationer.total
     unit="kr."
  %}
  </div>
  
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

