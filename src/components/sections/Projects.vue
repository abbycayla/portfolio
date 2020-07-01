<template>
<div>
  <!-- <div id="fullpage">
    <div class="section">
      <div class="slide" data-anchor="slide1"> Slide 1 </div>
	<div class="slide" data-anchor="slide2"> Slide 2 </div>
	<div class="slide" data-anchor="slide3"> Slide 3 </div>
	<div class="slide" data-anchor="slide4"> Slide 4 </div> -->
    <section id="projects">
    <h1> MY PROJECTS </h1>
    <div class="projects-list">
      <div class="project">
        <Arlo/>
        <BlackEstate/>
        <TravelBuddy/>
        <Wanderfy/>
      </div>
    </div>
  
  </section>
<!-- </div> -->
  </div>
</template>

<script>
import Arlo from '../projects/Arlo.vue'
import BlackEstate from '../projects/BlackEstate.vue'
import Wanderfy from '../projects/Wanderfy.vue'
import TravelBuddy from '../projects/TravelBuddy.vue'

export default {
  name: 'Projects',
  components: {
    Arlo,
    BlackEstate,
    Wanderfy,
    TravelBuddy
  }
}


</script>

<style scoped>

  #projects{
    padding: 7%;

  }
/* 
  .projects-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  } */

  h1 {
    /* margin: 0px 100px; */
    padding: 0px 0px 50px 0px;
    text-align: right;
    color: #010206;
    /* color: orangered; */
    font-size: 5em;
    border-bottom: 1px #010206 solid;
}


  .project {
    /* padding: 50px; */
  }

</style>
