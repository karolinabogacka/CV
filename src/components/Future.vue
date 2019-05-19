<template>
  <div>
    <section>
    <h2>{{ content.title }}</h2>
    <p v-for="(item, index) in content.future" :key="index">{{ item }}</p>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Future',
  data() {
    return {
      content: {
        title: "Plany na przyszłość",
        future: [
          "W niedalekiej przyszłości chciałabym rozpocząć pracę jako Junior Frontend Developer.",
          "Zdaję sobie sprawę z tego, że będzie to wymagało dużego zaangażowania oraz czasu, ale jestem zdeterminowana, by osiągnąć cel."
        ]
      }
    }
  }  
}
</script>

<style scoped lang="scss">
h1, h2, h3, h4 {
  text-decoration: underline;
}
.underlined {
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
