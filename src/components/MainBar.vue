<template>
  <div class="main-bar">
    <div class="container-img">
        <img src="../assets/img/img2.jpg" alt="evariste's picture" id="author-img">
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
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.main-bar {
    padding: 15px;
    height: 100vh;
    background-image: linear-gradient(200deg, #eff5ee, #f1ebec);
}

#author-img {
    border-radius: 50%;
    width: 50%;
}
.container-img {
    margin-top: 10px;
    text-align: center;
    margin-bottom: 20px;
}

.container-anchor {
    display: grid;
}

.container-anchor a {
    text-decoration: none;
    justify-self: center;
    font-size: 25px;
    font-weight: bold;
    margin: 10px 0px;
    font-family: 'Teko', sans-serif;
    transition: all 0.3s ease;
}
a:hover {
    width: 120px;
    text-align: center;
    background-color: rgb(73, 68, 64);
    color: #eff5ee;   
}

</style>

