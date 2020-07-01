<template>
  <div>
    <section id="contact">
      <div class="contact-content">
            <h1> CONTACT </h1>
            <div class="contact-links">
            <div class="media-links">

            </div>
            <div class="behance">
              <!-- <div>  -->
                <button> Visit my Behance Profile for more projects! </button>
              <!-- </div> -->
              <!-- <div>
               <img src="https://i.ibb.co/1QnKb3t/behance.png" alt="behance">
              </div> -->
            </div>
            <!-- </div> -->
            <div class="form">
            <form>
                <label> First name: </label> <br>
                <input type="text" name="firstname" placeholder="Name">
                <br>
                <label> Email: </label> <br>
                <input type="text" name="lastname" placeholder="Email">
                <br>
                <label> Message: </label> <br>
                <textarea rows="4" cols="50" placeholder="Message..."></textarea>
                <br>
                <input type="submit" value="Submit">
              </form> 
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
    /* border-bottom: 1px #010206 solid; */
}

.behance {
  display: flex;
  justify-content: center;
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
/* .behance img {
  width: 100%;
} */

</style>
