<template>
    <div>
        <section id="travel">

            <div class="travel-content">
                    <div class="travel-image">
                        <img src="https://i.ibb.co/P46cvjR/travel-min.png" alt="travel" v-on:click="on()">
                    </div>
            </div>       

            <div id="popup-travel">
                <div id="popup-content">
                    <div class="popup-text">
                        <h2> Travel Buddy </h2>
                        <p> This website, Travel Buddy, was created in 2019 in Level 6 Web and UX. Travel Buddy is a single page web application that allows users to search for accommodation in Christchurch. </p>
                        <div class="buttons">
                            <button> <a href="https://travel-buddy.netlify.app/" target="_blank"> View Live Site </a> </button>
                            <button> <a href="https://www.behance.net/gallery/96790497/Travel-Buddy" target="_blank"> UX Process </a> </button>
                        </div>
                    </div>

                    <div class="popup-image">
                        <img src="https://i.ibb.co/P46cvjR/travel-min.png" alt="travel">
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
  name: 'TravelBuddy',
  methods: {
    on: function() {
    document.getElementById("popup-travel").style.display = "block";
},

off: function() {
  document.getElementById("popup-travel").style.display = "none";
}
  }
}
</script>

<style scoped>

#travel {
    width: 100%;
    padding: 10%;
}

#travel:hover  {
    padding: 3%;
    transition: 0.4s;
    /* background-color: #010206; */
    cursor: pointer;
}

#popup-travel {
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
    background-image: linear-gradient(0deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.8)),url('https://i.ibb.co/P46cvjR/travel-min.png');
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
    cursor: pointer;
}

.travel-image img {
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

@media (max-width: 800px){

#travel {
    width: 100%;
    /* display: block; */
}

.travel-content {
    /* background-color: #101C31; */
    /* display: flex;
    justify-content: space-between; */
    background-image: url('https://i.ibb.co/LdKhDm8/travel.png');
    /* background-image: url('https://i.ibb.co/nkTNFSm/travel.png'); */
    background-repeat: no-repeat;
    background-size: 100%;
    /* display: flex;
    justify-content: space-between; */
    /* background-color: white; */
    height: 60vh;
    position: relative;
    /* width: 100%; */
}

.travel-text {
    background-color: #010206;
    /* border-radius: 90px; */
    /* height: 100%; */
    /* width: 90%; */
    font-weight: lighter;
    font-size: 1.2em;
    /* margin: 20px; */
    /* text-align: center; */
    padding: 30px 60px 10px 60px;
    /* margin-left: 50%; */
    /* position: absolute; */
    /* top: 200px; */
    /* left: 29px; */
}

p {
    padding-top: 50px;
    color: white;

}

h2 {
    padding-top: 10px;
    font-size: 2em;
    color: red;
    /* text-align: center; */
}

.travel-image img {
    width: 100%;
    /* position: relative; */
}

button {
    padding: 20px 10px;
    /* margin: 10% 5% 10% 5%; */
    font-size: .9em;
    /* width: 100%; */
}

}



</style>
