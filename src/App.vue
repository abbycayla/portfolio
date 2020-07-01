<template>
  <div id="app">
    <link href="https://fonts.googleapis.com/css2?family=Titillium+Web:wght@300;400;600&display=swap" rel="stylesheet">
    <Header/>
    <Landing/>
    <div class="margin">
    <About/>
    <!-- <Skills/> -->
    <Projects/>
    </div>
    <Contact/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Landing from './components/sections/Landing.vue'
import About from './components/sections/About.vue'
// import Skills from './components/sections/Skills.vue'
import Projects from './components/sections/Projects.vue'
import Contact from './components/sections/Contact.vue'

export default {
  name: 'App',
  components: {
    Landing,
    About,
    // Skills,
    Header,
    Projects,
    Contact
  }
}
</script>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

body {
    background-color: #010206;
    /* font-family: 'PT Sans', sans-serif; */
    font-family: 'Titillium Web', sans-serif;
}

.margin {
  margin: 0px 100px;
  background-color: white;
}
</style>
