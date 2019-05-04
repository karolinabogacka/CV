<template>
  <div class="hello">
    <section>
      <h1>{{ msg }}</h1>
      <p v-for="(item, index) in experience" :key="index"><b>{{ index + 1 }})</b> {{ item }}</p>
    </section>
    <section>
      <h2>{{ testingExperienceTitle }}</h2>
      <p v-for="(item, index) in testingExperience" :key="index"><b>{{ index + 1 }})</b> {{ item }}</p>
    </section>
    <section>
      <h3>LinkedIn</h3>
      <a href="https://www.linkedin.com/in/karolina-bogacka-289292163/" target="_blank" rel="noopener">Link</a>
    </section>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      experience: [
        "Własna działalność gospodarcza - SPEDIA K.B. Karolina Bogacka, od 2011 r.",
        "Współwłaściciel w Greysoft Sp. z o. o., od 2017 r.",
        "Instruktor nauki jazdy kat. B, B1",
      ],
      testingExperienceTitle: "Doświadczenie w testowaniu oprogramowania",
      testingExperience: [
        "Szkolenie indywidualne - tester manualny - teoria i praktyka - Waldemar Szafraniec",
        "Szkolenie przygotowujące do egzaminu ISTQB FL wraz z ćwiczeniami praktycznymi - Testuj.pl",
        "Szkolenie teoretyczne - Wstęp do pracy na stanowisku Tester Manualny - Anna Pieciulko-Czyrko",
        "Certyfikat ISTQB FL"
      ]
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
