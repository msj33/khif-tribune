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

  <div>
  {% include progressbar.html
     belob=site.data.donationer.belob
     total=site.data.donationer.total
     unit="kr."
  %}
  </div>

    <p>Opdatering 30 Maj: Tribunen er nu færdig! 🏟️ - Vi har dertil fået bygget ekstra 30 sæder gennem salg af 30 stk. sæde-sponsorater samt 2 sponsor-tilskud 👏</p>
    <br>
    <p>💚 Tusind tusind tak til alle jer der støtter dette fællesskabende projekt 💚</p>
    <br>
    <p>Nedenfor ses det færdige resultat af en tribune med i alt 120 sæder</p>
    <br>
    <p>Her i Juni måned afholdes der indvielse og åbent hus.....nærmere info følger snarest her og på sociale medier ⚽</p>

  <img src="{{ '/assets/tribune-1.jpg' | relative_url }}" alt="Ny tribune" class="tribune-image">
  <img src="{{ '/assets/tribune-2.jpg' | relative_url }}" alt="Ny tribune" class="tribune-image">
  <img src="{{ '/assets/tribune-3.jpg' | relative_url }}" alt="Ny tribune" class="tribune-image">

  <!-- Kursiv note før billedet -->
  <p style="font-size: 0.9em; font-style: italic; color: #ddd;">
    *Den oprindelige Ide-skitse til projektet*
  </p>

  <img src="{{ '/assets/khif_tribune-2.jpg' | relative_url }}" alt="Ny tribune" class="tribune-image">

  <p class="last-updated">
    Sidst opdateret: {{ site.data.donationer.sidst_opdateret }}
  </p>
</div>

