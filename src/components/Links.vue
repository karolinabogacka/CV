<template>
  <div class="hello">
    <section>
      <h2>Links</h2>
      <a href="https://www.linkedin.com/in/karolina-bogacka-289292163/" target="_blank" rel="noopener">LinkedIn</a>
      <a href="https://github.com/karolinabogacka/CV" target="_blank" rel="noopener">GitHub</a>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Links'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
  margin-bottom: 50px;
}
h1, h2, h3, h4 {
  text-decoration: underline;
}
a {
  display: block;
  margin: 10px;
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
