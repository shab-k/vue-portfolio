<template>
  <div class="wrapper">
    <!-- Photo(s) by 8biticon.com -->
      <About />
      <Skills />
      <Projects />
      <Contact />
  </div>
</template>

<script>
import About from '../components/About'
import Skills from '../components/Skills'
import Projects from '../components/Projects'
import Contact from '../components/Contact'

export default {
  name: 'Home',
  components: {
    About,
    Skills,
    Projects,
    Contact
  }
}
</script>
<style lang="scss">
</style>
