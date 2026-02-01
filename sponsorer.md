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
  Solgte reklameskilte
  </h2>

<div class="homepage-container">
  {% include progressbar.html
     belob=site.data.donationer.sponsorbelob
     total=site.data.donationer.sponsortotal
     unit="stk."
  %}
</div>
  
<h2 style="text-align: center; margin-top: 3rem;">
  Reklamesponsorer
</h2>

<div class="sponsor-grid">
  {% for sponsor in site.data.sponsorer %}
    <div class="sponsor-card">
      <div class="sponsor-navn">{{ sponsor.navn }}</div>
      <img src="{{ sponsor.logo | relative_url }}" alt="{{ sponsor.navn }}">
      <div class="sponsor-belob">
        {{ sponsor.belob }}
      </div>
    </div>
  {% endfor %}
</div>
