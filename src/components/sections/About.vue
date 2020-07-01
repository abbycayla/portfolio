<template>
   <div id="about">
            <div class="about-content">
                <div class="about-img">
                    <div>
                        <img src="https://i.ibb.co/5FZd0Wr/received-230208798045679.jpg" alt="profile-image">
                    </div>
                </div>
                <div class="about-info">
                <h1> ABOUT ME </h1>
                    <h3> I am currently studying Web and Ux design. I have studied design and web dev for 2 years now and have been wanting to pursue a career in the development industry from a young age. Check out my work and let me know what you think!</h3>
                    <div class="about-buttons">
                    <button> View My Work </button>
                    <button> Contact me </button>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style scoped>

#about {
    /* background-color: white; */
    /* margin: 0px 100px; */
        /* border-bottom: 1px #010206 solid; */
    background-image: linear-gradient(0deg, rgba(255, 255, 255, 0.9), rgba(255, 255, 255, 0.9)),url('https://i.ibb.co/dJNhc85/105705784-862249240939409-5464698221254601992-n.jpg');
    background-repeat: no-repeat;
    background-size: 100%;

}

.about-content {
    display: flex;
    justify-content: space-between;
    height: 100%;
    padding:  10% 7%;
}

.about-buttons {
    display: flex;
    justify-content: flex-end;
}

.about-info {
    width: 50%;
    background-image:url('')
    /* margin-top: 5%; */
}

  h1 {
    /* margin: 0px 100px; */
    /* padding: 70px 0px 50px 0px; */
    text-align: right;
    color: #010206;
    /* color: orangered; */
    font-size: 5em;
    /* border-bottom: 1px #010206 solid; */
}


.about-info h3{
    color: #010206;
    font-weight: 400;
    text-align: right;
    /* padding-top: 7%; */
    padding: 12% 0% 12% 12%;
    line-height: 1.8;
    font-size: 1.9em;
    margin: 0;
}

.about-content img {
    width: 100%;
    border-radius: 50%;
    margin-top: 5%; 
    /* padding-top: 20%; */
}


/* BUTTONS  */
button {
    background-color: #FF7D00;
    color: white;
    padding: 20px 30px;
    border: none;
    margin: 0% 0% 10% 10%;
    font-size: 1.5em;
    font-weight: 300;
}

button:hover {
    background-color: #010206;
    cursor: pointer;
}


 /* RESPONSIVENESS */

@media (max-width: 800px){

.about {
    margin: 0;
}

.about-content {
     flex-direction: column;
    align-items: center;
}

.about-content img {
    width: 40%;
}

h1 {
    margin-bottom: 0px;
    font-size: 2.2em;
}

.about-info {
    width: 100%;
    padding: 0px 50px;
    text-align: center;
}

.about-buttons {
    display: flex;
}
    
button {
    padding: 30px 10px;
    margin: 20% 5% 10% 5%;
    font-size: 1.3em;
    width: 100%;
}

.about img {
    width: 90%;
    display: block;
    margin: 30px auto 30px auto;
}
}
</style>


