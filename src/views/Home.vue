<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/Foto.jpg"><br/>
    <h1><i><b>Karolina Bogacka</b></i></h1><br/>
    <b>Miasto:</b> Gdańsk<br/>
    <b>Email:</b> kbogacka1@wp.pl<br/>
    <i><b>Telefon:</b> 535 365 341</i><br/>
    <p>Poszukuję pierwszej pracy/stażu (także bez płatnego)/praktyk, na stanowisku Junior Software Manual Tester</p>

    <HelloWorld msg="Doświadczenie zawodowe"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Experience from '@/components/Experience.vue'

export default {
  name: 'home',
  components: {
    HelloWorld: Experience
  }
}
</script>
