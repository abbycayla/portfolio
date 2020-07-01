<template>
  <div>
    <section id="landing">
        <div class="typewriter">
            <div class="typewriter-container">
                <h1> Hey! I'm Abby and I develop stuff </h1>
                <p> Scroll down to see more about me </p>
            </div>
        </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Landing',
}
</script>

<style scoped>

#landing {
    /* background: url(/images/flower.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: bottom; */
    /* overflow: hidden; */
    /* color: #FFFFFF;
    height: 100vh; */
}

.typewriter {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    background-image: linear-gradient(0deg, rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.9)),url('https://i.ibb.co/dJNhc85/105705784-862249240939409-5464698221254601992-n.jpg');
    background-repeat: no-repeat;
    background-size: 100%;
}

.typewriter-container {
    margin-top: 26%;
}

.typewriter h1 {
    color: #fff;
    overflow: hidden; 
    border-right: .15em solid orange;
    white-space: nowrap; 
    margin: 0 auto;
    letter-spacing: .15em;
    font-size: 4em;
    animation: 
      typing 3.5s steps(30, end),
      blink-caret .3s step-end infinite;
  }

.typewriter p {
    text-align: center;
    padding-top: 40%;
    font-size: 1.2em;
    margin-bottom: 2%;
}
  
  /* The typing effect */
@keyframes typing {
    from { width: 0 }
    to { width: 100% }
}
  
  /* The typewriter cursor effect */
@keyframes blink-caret {
    from, to { border-color: transparent }
    50% { border-color: orange }
}

 /* RESPONSIVENESS */

@media (max-width: 800px){
    #landing {
    height: 100%;
    }
    
    .typewriter {
        /* padding: 5% 0% 5% 0%; */
        height: 100vh;
        background-size: cover;
    }

    .typewriter-container {
        margin-top: 60%;
}

    .typewriter h1 {
        font-size: 2em;
    }

    .typewriter p {
        padding-top: 64%;
    }
}
</style>
