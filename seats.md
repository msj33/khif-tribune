---
layout: default
title: "Sponsorsæde"
---

# Køb af tribunesæde 💚⚽️🏟

Vil du være en del af KHIF-historien? Nu har du chancen for at sikre dig et **tribunesæde med dit eget navn/firmanavn** på vores nye tribune! For **500 kr.** kan du:

- Få dit navn påtrykt på ét af de 90 unikke sæder.
- Være med til at vise din støtte til byggeriet af tribunen og samtidig skabe **bedre fællesskab og rammer** for vores lokale klub.  
- Være en del af et minde - Sædet har en historie fra det tidligere Aarhus Stadion i perioden 1999-2025

*Sponsoratet er udelukkende navngivende og giver ikke særlige rettigheder til sædet.*

<h2 style="text-align: center; margin-bottom: 10px;">
  UDSOLGT - Solgte sæder - UDSOLGT
  </h2>

<div class="homepage-container">
  {% include progressbar.html
     belob=site.data.donationer.seatbelob
     total=site.data.donationer.seattotal
     unit="stk."
  %}
</div>

<h2 style="text-align: center; margin-top: 3rem;">
  Solgte Tribune Sæder
</h2>


<div class="seats-grid">
  {% for seat in site.data.saeder %}
    <div class="seat-card">
      <img src="{{ '/assets/saedeskilt.jpg' | relative_url }}" alt="Tribunesæde">
      <div class="seat-name">
        {{ seat.seat }}
      </div>
    </div>
  {% endfor %}
</div>

  
<img src="{{ '/assets/seats.png' | relative_url }}" alt="Seats" class="fonde-image">
