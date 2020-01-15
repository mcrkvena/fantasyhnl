<template>
  <div class="jumbotron jumbotron-fluid" style="padding: 0.5em; background-image: url(ademi.jpg); background-repeat:no-repeat; background-size:90%; height: 900px; background-position: 50% 50%">
    <h1 class="display-2" style="font-family:Impact; text-align:left; color: white; margin-left: 110px;"><b>BUDI I TI DIO EKIPE</b></h1>
    <h2 style="text-align:left; font-family:Impact; margin-left:420px; margin-top:60px; margin-bottom:30px;"><router-link v-if="!authenticated" class="btn btn-info" style="font-size:72px; opacity:0.8; text-shadow:2px 2px black;" to="/login">Prijavi se</router-link></h2>
    <p style="text-align:left; font-family:Consolas; margin-left:432px; color:#85e0e0; font-size:20px;">ili, ako si novi korisnik</p>
    <h2 style="text-align:left; font-family:Impact; margin-left:420px; margin-top:30px;"><router-link v-if="!authenticated" class="btn btn-info" style="font-size:72px; opacity:0.8; text-shadow:2px 2px black;" to="/register">Registriraj se</router-link></h2>
  </div>
</template>


