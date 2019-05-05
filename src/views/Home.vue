<template>
  <div class="home">
    <Header/>
    <Experience msg="Doświadczenie zawodowe"/>
    <Links/>
  </div>
</template>

<script>
// @ is an alias to /src
import Experience from '@/components/Experience.vue'
import Header from '@/components/Header.vue'
import Links from '@/components/Links.vue'

export default {
  name: 'home',
  components: {
    Experience: Experience,
    Header: Header,
    Links: Links
  }
}
</script>
