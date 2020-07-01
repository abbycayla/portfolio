<template>
  <div>
    <section id="contact">
      <div class="contact-content">
            <div class="contact-links">
              <div>
                <img class="profile-image" src="https://i.ibb.co/5FZd0Wr/received-230208798045679.jpg" alt="profile-image">
              </div>
              <div>
            <h1> CONTACT </h1>
              <p> If you are interested in my work and want to get in contact with me you can do so via the links below or email me at </p>
              <a class="email-link" href="mailto:abbycloete3552@gmail.com "> abbycloete3552@gmail.com </a>
            <div class="media-links">
              <a href="https://www.instagram.com/abbythecayla/?hl=en"><img src="https://i.ibb.co/9tmnBMr/instagram-1.png" alt="instagram-1" border="0"></a>
              <a href="https://twitter.com/_sushifish"><img src="https://i.ibb.co/MCFD2ZK/twitter-1.png" alt="twitter-1" border="0"></a>
              <a href="https://github.com/abbycayla"><img src="https://i.ibb.co/VBrGCWZ/Git-Hub-Mark-Light-64px.png" alt="Git-Hub-Mark-Light-64px" border="0"></a>
            </div>
            <div class="behance">
            <h2> Visit my Behance Profile for more of my work </h2>
            <button> <a href="https://www.behance.net/abbycloete" target="_blank"> My Behance </a> </button>
            </div>
            </div>
            </div>
        </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Contact'
}
</script>

<style scoped>

#contact {
    background-image: linear-gradient(0deg, rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.9)),url('https://i.ibb.co/dJNhc85/105705784-862249240939409-5464698221254601992-n.jpg');
    background-repeat: no-repeat;
    background-size: 100%;
    height: 100vh;
}

.form {
    display: flex;
    justify-content: flex-end;
    padding-bottom: 10%;
    margin-right: 13%;
}

input, textarea{
    padding: 10px 20px;
    margin: 20px 0px;
    width: 400px;
}

label {
    color: white;
    font-size: 1.2em;

}

.contact-content {
    padding:  7% 7%;

}

 h1 {
    /* margin: 0px 100px; */
    /* padding: 70px 0px 50px 0px; */
    text-align: right;
    color: white;
    /* color: orangered; */
    font-size: 5em;
    margin-bottom: 5%;
    border-bottom: 1px white solid;
}

/* .behance {
  display: flex;
  justify-content: center;
} */

.contact-links {
  padding: 5% 0%;
  display: flex;
}

.profile-image {
    border-radius: 50%;
    /* width: 200px; */
    margin-top: 7%;

}

.media-links {
  display: flex;
  justify-content: flex-end;
  margin: 5% 0%
}

.media-links img{
  width: 70px;
}

.media-links a {
  margin-left: 2%;
}

.contact-links p {
  color: white;
  font-size: 2em;
  text-align: right;
  font-weight: lighter;
  margin-left: 20%;
}

.email-link {
  color: #FF7D00;
  font-size: 2.2em;
  text-decoration: none;
  margin-left: 57%;
  /* font-weight: lighter; */
  text-align: right;
}

.contact-links h2 {
  color: white;
  text-align: right;
  font-size: 1.6em;
}

.behance {
  /* width: 30%; */
}

button {
    background-color: #FF7D00;
    padding: 20px 30px;
    border: none;
    margin: 3% 0% 0% 50%;
    width: 50%;
    /* display: block; */
    /* margin-right: 0; */
    /* margin-left: 50%; */
}

button a {
    color: white;
    font-size: 2em;
    font-weight: 300;
    text-decoration: none;
}

button:hover {
    background-color: white;
    cursor: pointer;
}

button a:hover {
  color: #FF7D00;
}
/* .behance img {
  width: 100%;
} */

</style>
