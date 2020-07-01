<template>
    <div>
        <section id="wanderfy">

            <div class="wanderfy-content">
                    <div class="wanderfy-image">
                        <img src="https://i.ibb.co/mHCTxSq/79206304-272494084019245-6525036843091195611-n.png" alt="wanderfy" v-on:click="on()">
                    </div>
            </div>

            <div id="popup-wanderfy">
                <div id="popup-content">
                    <div class="popup-text">
                        <h2> Wanderfy App </h2>
                        <p> This is an app prototype for a custom made app called Wanderfy, created in Level 5 Web and Graphic 2019. This app is a fun way help teens and young adults get out and about in Christchurch using Wanderfy which gives you in-app rewards for visiting certain activity points in Christchurch </p>
                        <div class="buttons">
                            <button> <a href="https://projects.invisionapp.com/d/main?origin=v7#/console/17143445/357207812/preview?scrollOffset=620" target="_blank"> View Live Prototype </a> </button>
                            <button> <a href="https://www.behance.net/gallery/96791945/Wanderfy-Group-App-Mockup" target="_blank"> UX Process </a> </button>
                        </div>
                    </div>

                    <div class="popup-image">
                        <img src="https://i.ibb.co/mHCTxSq/79206304-272494084019245-6525036843091195611-n.png" alt="wanderfy">
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
  name: 'Wanderfy',
  methods: {
    on: function() {
    document.getElementById("popup-wanderfy").style.display = "block";
},

off: function() {
  document.getElementById("popup-wanderfy").style.display = "none";
}
  }
}
</script>

<style scoped>

#wanderfy {
    width: 100%;
    padding: 10%;
}

#wanderfy:hover  {
    padding: 5%;
    transition: 0.4s;
    background-color: #010206;
    cursor: pointer;
}

#popup-wanderfy {
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
    background-image: linear-gradient(0deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0.8)),url('https://i.ibb.co/mHCTxSq/79206304-272494084019245-6525036843091195611-n.png');
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

.wanderfy-image img {
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

#wanderfy {
    width: 100%;
    /* display: block; */
}

.wanderfy-content {
    /* background-color: #101C31; */
    /* display: flex;
    justify-content: space-between; */
    background-image: url('https://i.ibb.co/LdKhDm8/wanderfy.png');
    /* background-image: url('https://i.ibb.co/nkTNFSm/wanderfy.png'); */
    background-repeat: no-repeat;
    background-size: 100%;
    /* display: flex;
    justify-content: space-between; */
    /* background-color: white; */
    height: 60vh;
    position: relative;
    /* width: 100%; */
}

.wanderfy-text {
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

.wanderfy-image img {
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
