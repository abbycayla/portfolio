<template>
    <div>
        <section id="blackestate">

            <div class="blackestate-content">
                    <div class="blackestate-image">
                        <img src="https://i.ibb.co/kGmRyy9/1.png" alt="blackestate" v-on:click="on()">
                    </div>
            </div>

            <div id="popup-be">
                <div id="popup-content">
                    <div class="popup-text">
                        <h2> Black Estate</h2>
                        <p> This website for the Black Estate was created in 2019 during Level 6 Web and UX at Yoobee Colleges. Black Estate is a remake of the original Black Estate site. </p>
                        <div class="buttons">
                            <button> <a href="https://black-estate-remake.netlify.app/" target="_blank"> View Live Site </a> </button>
                            <button> <a href="https://www.behance.net/gallery/96795743/Black-Estate-Redesign" target="_blank"> UX Process </a> </button>
                        </div>
                    </div>

                    <div class="popup-image">
                        <img src="https://i.ibb.co/kGmRyy9/1.png" alt="blackestate">
                    </div>

                    <div>
                        <button class="close-popup" v-on:click="off()"> X </button>   
                    </div>
                </div>
            </div>

        </section>
    </div>
</template>

<script>
export default {
  name: 'BlackEstate',
  methods: {
    on: function() {
    document.getElementById("popup-be").style.display = "block";
},

off: function() {
  document.getElementById("popup-be").style.display = "none";
}
  }
}
</script>

<style scoped>

#blackestate {
    width: 100%;
    padding: 10%;
}

#blackestate:hover  {
    padding: 3%;
    transition: 0.4s;
    /* background-color: #010206; */
    cursor: pointer;
}

#popup-be {
    position: fixed;
    display: none;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: rgba(0,0,0,0.7);
    z-index: 2;
    cursor: pointer;
}

#popup-content{
    position: absolute;
    display: flex;
    justify-content: space-between;
    top: 50%;
    left: 50%;
    padding: 20px;
    width: 80%;
    transform: translate(-50%,-50%);
    -ms-transform: translate(-50%,-50%);
    background-image: linear-gradient(0deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.8)),url('https://i.ibb.co/kGmRyy9/1.png');
    background-repeat: no-repeat;
    background-size: 100%;
}

.popup-image {
    padding: 15% 5%;
}

.popup-text {
    padding: 7% 5%;
    color: #010206;
}

h2 {
    font-size: 5em;
    font-weight: 600;
    padding-bottom: 20px;
}

p {
    font-size: 2em;
    font-weight: 400;
}

.close-popup {
    border-radius: 10px;
    width: 50px;
    text-align: center;
    font-size: 3em;
    color: white;
    margin: 0;
    top: 50px;
    right: 50px;
    padding: 0;
    position: absolute;
}

.blackestate-image img {
    width: 100%;
}

button {
    background-color: #FF7D00;
    padding: 20px 30px;
    border: none;
    margin: 10% 10% 0% 0%;
    width: 210px;
}

button a {
    color: white;
    font-size: 1.7em;
    font-weight: 300;
    text-decoration: none;
}

button:hover {
    background-color: #010206;
    cursor: pointer;
}



</style>
