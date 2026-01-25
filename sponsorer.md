---
layout: default
title: "Sponsorer"
---

# Bliv reklamesponsor

Som en del af finansieringen af KHIF Tribunen udbydes der 12 reklamesponsorpladser.

Reklameskiltene opsættes på den øverste langside ved tribunen.

Prisen for et reklameskilt er samlet 5.000 kr. excl. moms og løber over en 5-årig periode og betales up front. Fradragsberettiget for erhverv.  

Brug “Kontakt os” i menuen til venstre, hvis du ønsker at blive reklamesponsor i KHIF Fodbold.

<h2 style="text-align: center; margin-bottom: 10px;">
  Solgte Reklameskilte
  </h2>

<div class="homepage-container">
  {% include progressbar.html
     belob=site.data.donationer.sponsorbelob
     total=site.data.donationer.sponsortotal
     unit="stk."
  %}
</div>
  
<h2 style="text-align: center; margin-top: 3rem;">
  Reklamesponsorpladser
</h2>

<div class="sponsor-grid">
  {% for i in (1..12) %}
  <div class="sponsor-card">
    <img src="{{ '/assets/bsas.jpg' | relative_url }}" alt="Sponsor">
    <div class="sponsor-belob">
      18.500 kr.
    </div>
  </div>
  {% endfor %}
</div>
