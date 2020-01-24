---
layout: page
title: PROGRAMAÇÃO
permalink: /programação/
---
<!-- nao mexer -->
<table class="days" style="width:100%">
  <tr>
    <td class="segunda" onclick="selectDay('segunda')">SEGUNDA</td>
    <td class="terca" onclick="selectDay('terca')">TERCA</td>
    <td class="quarta" onclick="selectDay('quarta')">QUARTA</td>
    <td class="quinta" onclick="selectDay('quinta')">QUINTA</td>
    <td class="sexta" onclick="selectDay('sexta')">SEXTA</td>
    <td class="sabado" onclick="selectDay('sabado')">SABADO</td>
    <td class="domingo" onclick="selectDay('domingo')">DOMINGO</td>
  </tr>
</table>
<!-- nao mexer -->
<div class="prog">
  <div class="segunda">
  <img src="/imagens/" mhhhhhgfggg.png alt="MÚSIC NONSTOP">
  <img src="/imagens/" alt="">
  <img src="/imagens/.png" alt="">
  <img src="/imagens/" alt="">
  <img src="/imagens/m .png" alt="">
  </div>
  <div class="terca">
    <img src="/imagens/music-nonstop.png" alt="MUSIC NONSTOP">
    <img src="/imagens/meiahorasempausas.png" alt="MEIA HORA SEM PAUSAS">
    <img src="/imagens/random .png" alt="RANDOM">
    <img src="/imagens/fantassummer.png" alt="FANTAS SUMMER">
    <img src="/imagens/out night .png" alt="OUT NIGHT">
  </div>
  <div class="quarta">
    <img src="/imagens/music-nonstop.png" alt="MUSIC NONSTOP">
    <img src="/imagens/meiahorasempausas.png" alt="MEIA HORA SEM PAUSAS">
    <img src="/imagens/random .png" alt="RANDOM">
    <img src="/imagens/fantassummer.png" alt="FANTAS SUMMER">
    <img src="/imagens/out night .png" alt="OUT NIGHT">
  </div>
  <div class="quinta">
    <img src="/imagens/music-nonstop.png" alt="MUSIC NONSTOP">
    <img src="/imagens/meiahorasempausas.png" alt="MEIA HORA SEM PAUSAS">
    <img src="/imagens/random .png" alt="RANDOM">
    <img src="/imagens/fantassummer.png" alt="FANTAS SUMMER">
    <img src="/imagens/out night .png" alt="OUT NIGHT">
  </div>
  <div class="sexta">
    <img src="/imagens/music-nonstop.png" alt="MUSIC NONSTOP">
    <img src="/imagens/davidegaspar11 .png" LUCH TIME>
    <img src="/imagens/random .png" alt="RANDOM">
    <img src="/imagens/fantassummer.png" alt="FANTAS SUMMER">
    <img src="/imagens/out night .png" alt="OUT NIGHT">  
  </div>
  <div class="sabado">
    <img src="/imagens/feelthemusic .png" alt="FEEL THE MÚSIC">
    <img src="/imagens/musicnonstop1 .png" alt="MUSIC NONSTOP">
    <img src="/imagens/musicboxcomsaracorreia2 .png" alt="Sara Correia">
    <img src="/imagens/2hsempausas2.png" alt="2H SEM PAUSAS">
    <img src="/imagens/meiahorasempausas2.png" alt="MEIA HORA SEM PAUSAS">
    <img src="/imagens/web9.png" alt="WEB 9">
    <img src="/imagens/nunoreis.png" alt="Nuno Reis">
    <img src="/imagens/danielgaspar.png" alt="Daniel Gaspar">

  </div>
  <div class="domingo">
    <img src="/imagens/housepartyradioshow.png" alt="HOUSEPARTYRADIOSHOW">
    <img src="/imagens/musicnonstop1 .png" alt="MUSIC NONSTOP">
    <img src="/imagens/saracorreia 33 .png" alt="Sara Correia">
    <img src="/imagens/2hsempausas2.png" alt="2H SEM PAUSAS">
    <img src="/imagens/meiahorasempausas2.png" alt="MEIA HORA SEM PAUSAS">
    <img src="/imagens/web9.png" alt="WEB 9">
    <img src="/imagens/danielgaspar2.png" alt="Daniel Gaspar">
  </div>
</div>

<!-- nao mexer -->
<script>
  var allDays = document.querySelectorAll('.days tr td');
  var allProg = document.querySelectorAll('.prog div');
  function selectDay(day){
    var selectedDay = document.querySelector('.days tr td.'+day);
    var selectedProg = document.querySelector('.prog div.'+day);
    for (var i = 0; i < allDays.length; i++) {
      allDays[i].classList.remove('selected');
      allProg[i].classList.remove('selected');
    }
    selectedDay.classList.add('selected');
    selectedProg.classList.add('selected');
  }
  var today = new Date().getDay();
  var dayOfTheWeek = today === 0 ? 6 : today-1;
  allProg[dayOfTheWeek].classList.add('selected');
  allDays[dayOfTheWeek].classList.add('selected');
</script>
<style>
  .days tr td{
    border: 0;
    text-align: center;
    font-weight: bold;
    cursor: pointer;
    color: black;
    background-color: none;
  }
  .days tr td.selected{
    color: white;
    background-color: #0092ca;
  }
  .prog div{
    display: none;
  }
  .prog div.selected{
    display: block;
  }
</style>
<!-- nao mexer -->
