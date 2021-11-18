---
layout: page
title: PROGRAMAÇÃO
permalink: /programacao/
---

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

<div class="prog">
  <div class="segunda">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  <img src="/imagens/.png" alt="A TARDE">
  <img src="/imagens/.png" alt="DANCE MÚSIC">

  </div>
  <div class="terca">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  <img src="/imagens/.png" alt="A TARDE">


  </div>
  <div class="quarta">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  <img src="/imagens/.png" alt="A TARDE">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">



  </div>
  <div class="quinta">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  <img src="/imagens/a-tarte1.png" alt="A TARDE">

  </div>
  <div class="sexta">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  <img src="/imagens/.png" alt="A TARDE">
  <img src="/imagens/.png" alt="A NOITE">

  </div>
  <div class="sabado">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  <img src="/imagens/.png" alt="MÚSICA SEM PARAR">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  </div>
  <div class="domingo">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
  <img src="/imagens/.png" alt="MÚSICA SEM PARAR">
  <img src="/imagens/.png" alt="MUSIC NONSTOP">
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
