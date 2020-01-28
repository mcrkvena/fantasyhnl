<template>
  <div class="jumbotron jumbotron-fluid" id="jumbo1" style="background-image: url(ademi.jpg);">
    <h1 class="display-2" id="naslovhome"><b>BUDI I TI DIO EKIPE</b></h1>
    <h2 id="log"><router-link v-if="!authenticated" class="btn btn-info" id="tipkahome" to="/login">Prijavi se</router-link></h2>
    <p id="ili">ili, ako si novi korisnik</p>
    <h2 id="reg"><router-link v-if="!authenticated" class="btn btn-info" id="tipkahome" to="/register">Registriraj se</router-link></h2>
  </div>
</template>

<style>
  #jumbo1{
    padding: 0.5em;
    background-repeat:no-repeat;
    background-size:cover;
    height:900px;
    background-position: 50% 50%;
  }
  #naslovhome{
    font-family:Impact;
    text-align:left;
    color: white;
    margin-left: 4%;
  }
  #log{
    text-align:left;
    font-family:Impact;
    margin-left:22.5%;
    margin-top:60px;
    margin-bottom:30px;
  }
  #ili{
    text-align:left;
    font-family:Consolas;
    margin-left:22.75%;
    color:#85e0e0;
    font-size:20px;
  }
  #reg{
    text-align:left;
    font-family:Impact;
    margin-left:22.5%;
    margin-top:30px;
  }
  #tipkahome{
    font-size:72px;
    opacity:0.8;
    text-shadow:2px 2px black;
  }
</style>