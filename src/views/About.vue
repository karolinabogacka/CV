<template>
  <div class="about">
    <h1>Kilka słów o mnie</h1>
    <p v-for="(item, index) in experience" :key="index"><b>{{ index + 1 }})</b> {{ item }}</p>
    <h2>Kilka słów o mnie</h2>
    
    <section>
      <p>Od ponad 8 lat prowadzę działalność gospodarczą w branży telekomunikacja/IT.</p>
      <p>Tematem testowania oprogramowania oraz samym programowaniem, zainteresował mnie Mąż - programista z 19letnim stażem.</p>
      <p>Stawiam na ciągły rozwój, więc postanowiłam,że poza prowadzeniem własnej firmy, zacznę uczyć się rzeczy, którym do tej pory przyglądałam się z boku.</p>
      <p>Jestem osobą komunikatywną, otwartą, a dzięki dotychczasowym zajęciom zawodowym, posiadam duże doświadczenie w kontakcie z Klientem.</p>
    </section>

    <h1>Zainteresowania</h1>
    <section>
      <p>Uwielbiam książki, dobre filmy, motoryzację oraz spędzanie czasu na łonie natury.</p>
    </section>
  </div>
</template>

<style scoped lang="scss">
section {
  margin-bottom: 50px;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

