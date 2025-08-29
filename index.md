---
layout: default
title: "Forside"
---

<div class="homepage-container">
  <h1>Ny Tribune til Kolt-Hasselager IF</h1>

  <p>Vi samler ind til en ny tribune, som skal skabe fællesskab og give endnu bedre rammer for vores klub.</p>

  <div class="counter">
    Indsamlet beløb: <strong>{{ site.data.donationer.belob }} kr.</strong>
  </div>

  {% assign procent = site.data.donationer.belob | times: 100 | divided_by: 500000 %}

  <div class="progress-container">
    <div class="progress-bar" style="width: {{ procent }}%;"></div>
    <div class="progress-text">{{ site.data.donationer.belob }} kr. af 500.000 kr.</div>
  </div>

  <p>Se de støttende donorer og fonde i menuen til venstre.</p>

  <img src="/assets/khif_tribune.png" alt="Ny tribune">

  <p style="text-align: center; font-style: italic; color: #333333;">
    Sidst opdateret: {{ site.data.donationer.sidst_opdateret }}
  </p>
</div>

