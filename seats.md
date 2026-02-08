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
  UDSOLGT - UDSOLGT - Solgte sæder - UDSOLGT - UDSOLGT
  </h2>

<div class="homepage-container">
  {% include progressbar.html
     belob=site.data.donationer.seatbelob
     total=site.data.donationer.seattotal
     unit="stk."
  %}
</div>
  
💡 ## Solgte Tribune Sæder

{% assign seats = site.data.saeder %}
{% assign columns = 5 %}
{% assign rows = 18 %}
{% assign seat_index = 0 %}

| {% for c in (1..columns) %} | {% endfor %} |
| {% for c in (1..columns) %} --- | {% endfor %} |

{% for r in (1..rows) %}
|{% for c in (1..columns) %}
  {% assign seat = seats[seat_index] %}
  {% if seat %}
    {{ seat.navn }} 
  {% else %}
    &nbsp;
  {% endif %} |{% assign seat_index = seat_index | plus: 1 %}{% endfor %}
{% endfor %}
  
<img src="{{ '/assets/seats.png' | relative_url }}" alt="Seats" class="fonde-image">
