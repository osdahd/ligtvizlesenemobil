layout: default
title: "ligtvizlesene mobil | Canlı maç izle"
description: "Justin TV, Selçuk Sports HD, Taraftarium24, bedava maç izle mobil"
---
<div class="container">
  {% for match in site.data.matches %}
  <div class="match-card">
    <div class="match-header">
      <span class="match-time">{{ match.time }}</span>
      <span class="match-category">{{ match.category }}</span>
    </div>
    <div class="match-title">{{ match.teams }}</div>
    <button class="menu-btn">☰ Chaînes / Réseaux</button>
  </div>

  <div class="side-menu">
    <button class="close-btn">&times;</button>
    <a href="{{ match.kanal }}">📺 {{ match.channel_name }}</a>
    <hr>
    <a href="https://twitter.com/NazifSpor" class="twitter" target="_blank">Twitter</a>
    <a href="https://t.me/ligtvizlesene1" class="telegram" target="_blank">Telegram</a>
    <a href="https://discord.com/invite/4X6Bg8xNgG" class="discord" target="_blank">Discord</a>
  </div>
  {% endfor %}
</div>
