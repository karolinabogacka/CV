<template>
  <div class="about">
    <h2>Kilka słów o mnie</h2>
  
    <section>
      <p>Od ponad 8 lat prowadzę działalność gospodarczą w branży telekomunikacja/IT.</p>
      <p>Tematem testowania oprogramowania oraz samym programowaniem, zainteresował mnie Mąż - programista z 19letnim stażem.</p>
      <p>Stawiam na ciągły rozwój, więc postanowiłam,że poza prowadzeniem własnej firmy, zacznę uczyć się rzeczy, którym do tej pory przyglądałam się z boku.</p>
      <p>Jestem osobą komunikatywną, otwartą, a dzięki dotychczasowym zajęciom zawodowym, posiadam duże doświadczenie w kontakcie z Klientem.</p>
    </section>

    <h2>Zainteresowania</h2>
    <section>
      <p>Uwielbiam książki, dobre filmy, motoryzację oraz spędzanie czasu na łonie natury.</p>
    </section>
    <Future/>
    
  </div>
</template>

<script>
// @ is an alias to /src
import Future from '@/components/Future.vue'
export default {
  name: 'About',
  components: {
    Future: Future
  }
}
</script>

<style scoped lang="scss">
h1, h2, h3, h4 {
  text-decoration: underline;
}
section {
  margin-bottom: 50px;
}
h3 {
  margin: 40px 0 0;
}
a {
  color: #4268b9;
}
</style>

