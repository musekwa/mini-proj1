<template>
  <div class="main-bar">
    <div class="container-img">
        <img v-bind:src="img" alt="" id="author-img">
    </div>
    <div class="container-anchor">
        <router-link to="/"  id="about-btn">Quem Sou Eu?</router-link>
        <router-link to="/work" id="work-btn"> O que faço?</router-link>
        <router-link to="/hobbies" id="hobbies-btn">Hobbies</router-link>
    </div>
  </div>
</template>

<script>
/* eslint-disable */

export default {
  name: 'MainBar',
  data () {
    return {
      msg: 'Main Bar'
    }
  },
  img: '../assets/img.jpg',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Teko:wght@300&display=swap');
.main-bar {
    padding: 20px;
    color: white;
    height: 100vh;
    border: 6px solid green;
    background-image: linear-gradient(120deg, #11500f, #ff537f);
}

#author-img {
    border-radius: 50%;
    width: 100%;
}
.container-img {
    margin-top: 20px;
    text-align: center;
    margin-bottom: 20px;
}

.container-anchor {
    display: grid;
}

.container-anchor a {
    text-decoration: none;
    justify-self: center;
    color: rgb(196, 188, 188);
    font-size: 25px;
    margin: 10px 0px;
    font-family: 'Teko', sans-serif;
    transition: all 0.3s ease;
}
a:hover {
    width: 120px;
    text-align: center;
    background-color: rgb(66, 30, 5);
   
}

</style>

