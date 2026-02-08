---
layout: default
title: "Sponsorsæde"
---

# Hjælp med at få den sidste finansiering på plads – køb et tribunesæde 💚⚽️🏟

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

<!-- Grid med samme kode-logik som sponsorer, 5 kolonner × 18 rækker -->
<div class="sponsor-grid" style="grid-template-columns: repeat(5, 1fr);">
  {% assign seats = site.data.saeder %}
  {% assign total_slots = 5 | times:18 %}
  {% assign seat_index = 0 %}

  {% for i in (1..total_slots) %}
    {% assign seat = seats[seat_index] %}
    <div class="sponsor-card">
      {% if seat %}
        <div class="sponsor-navn">{{ seat.navn }}</div>
        {% if seat.billede %}
          <img src="{{ seat.billede | relative_url }}" alt="{{ seat.navn }}">
        {% else %}
          <img src="{{ '/assets/default-seat.png' | relative_url }}" alt="{{ seat.navn }}">
        {% endif %}
      {% else %}
        &nbsp; <!-- tom plads hvis der er færre end 90 sæder -->
      {% endif %}
    </div>
    {% assign seat_index = seat_index | plus: 1 %}
  {% endfor %}
</div>
  
<img src="{{ '/assets/seats.png' | relative_url }}" alt="Seats" class="fonde-image">
