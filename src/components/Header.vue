<template>
  <div>
    <section id="header">
    <h1> Header </h1>
    <nav>
      <ul>
          <li> <a href="#landing"> HOME </a> </li>
          <li> <a href="#about"> ABOUT ME </a> </li>
          <li> <a href="#projects"> MY PROJECTS </a> </li>
          <li> <a href="#contact"> CONTACT </a> </li>
      </ul>
    </nav>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped>
nav {
    top: 0;
    position: fixed;
    width: 100%;
}

nav ul{
    background-color: white;
    display: flex;
    justify-content: center;
    border-bottom: 2px solid #101C31;
    /* padding-top: 13px; */
    height: 100px;
}

li {
    list-style-type: none;
    padding: 30px 35px;
    font-size: 2em;
    font-weight: 700;
}

li a {
    text-decoration: none;
    color: #101C31;
}

li:hover {
    background-color: #FF7D00;
}

li a:hover {
    color: white;
}


@media (max-width: 800px){

  nav ul{
    height: 100px;
    padding-top: 20px;

  }

  li a {
    font-size: 1.2em;
  }

}

</style>
