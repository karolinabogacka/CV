<template>
  <div class="hello">
    <section>
      <h1>{{ msg }}</h1>
      <p class="ExperienceHeader">
        <span>Stanowisko</span>
        <span>Nazwa firmy</span>
        <span>Okres pracy</span>
      </p>
      <p v-for="(item, index) in experience" :key="index">
        <span>{{ item.type }}</span>
        <span>{{ item.name }}</span>
        <span>{{ item.period }}</span>
     </p>
    </section>
    <section>
      <h2>{{ testingExperienceTitle }}</h2>
      <p v-for="(item, index) in testingExperience" :key="index">
        <span>{{ item.type }}</span>
        <span>{{ item.name }}</span>
      </p>
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
        {
          type: "Własna działalność gospodarcza", 
          name: "SPEDIA K.B. Karolina Bogacka", 
          period: "od 2011 r."
        },
        { 
          type: "Współwłaściciel w spółce",
          name: "Greysoft Sp. z o. o.", 
          period: "od 2017 r."
        },
        {
          type: "Instruktor nauki jazdy kat. B, B1",
          name: "SPEDIA K.B. Karolina Bogacka",
          period: "od 2011 r."
        }
      ],
      testingExperienceTitle: "Doświadczenie w testowaniu oprogramowania",
      testingExperience: [
        {
          type: "Szkolenie indywidualne - tester oprogramowania - teoria + praktyka",
          name: "Waldemar Szafraniec"
        },
        {
          type: "Szkolenie przygotowujące do egzaminu ISTQB FL wraz z ćwiczeniami praktycznymi",
          name: "Testuj.pl"
        },
        {
          type: "Szkolenie teoretyczne - Wstęp do pracy na stanowisku Tester Manualny",
          name: "Anna Pieciulko-Czyrko"
        },
        {
          type: "Certyfikat ISTQB FL",
          name: "GASQ"
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

section {
  margin-bottom: 50px;
  border: 1px solid red;
}

h1, h2 {
  text-decoration: underline;
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

span {
  margin: 0 30px; 
  text-align: left;
  width: 250px;
  display: inline-block;
  border: 1px solid green;
}

.ExperienceHeader {
  font-weight: bold;
  text-transform: uppercase;
}
</style>
