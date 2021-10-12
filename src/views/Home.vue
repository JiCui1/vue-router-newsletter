<template>
  <div class="home" :style="{'background-image': 'url(' + require('../assets/bg.jpg') + ')'}">
    <div class="border">
      <h1 id="logo" href="/">Gamers</h1>
      <TextComp titleText='Black Myth Wukong'  description="Black Myth: Wukong (黑神话：悟空) is an upcoming
              action role-playing game by Chinese indie developer
              Game Science, based on the classical 16th-century 
              Chinese novel Journey to the West."/>
      <div class="img_container">
        <img src="../assets/game1.png" />
        <img src="../assets/game2.png" />
        <img src="../assets/game3.png" />
        <img src="../assets/game4.png" />
        <img src="../assets/game5.png" />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import TextComp from '../components/TextComp.vue'

export default {
  name: 'Home',
  components: {
    TextComp
  }
}
</script>

<style scoped>

#logo{
  color:white;
  text-align: left;
  font-weight: 900;
  margin-left:1rem;
  margin-top:1rem;
}

.text_container{
  text-align: left;
  color:white;
  margin-top: 6rem;
  margin-left:2rem;
}

.text_container h5{
  color:#F8CD7A;
  font-size:1.5rem;
  margin-bottom: -0.7rem;;
}

.text_container h1{
  font-size:3rem;
  font-weight: 900;
}

.text_container p{
  font-size: 1.2rem;
  line-height: 1.5;
  margin-top:1rem;
  font-weight: 500;
}

.text_container button{
  margin-top:2rem;
  width:6rem;
  height:2rem;
  border-radius: 20px;
  border:none;
  background: rgb(249,217,118);
  background: linear-gradient(90deg, rgba(249,217,118,1) 0%, rgba(243,159,134,1) 100%);
}

.home{
  width: 100%;
  height: 100vh;
  background-size:cover;
  display:flex;
  justify-content: center;
  align-items: center;
  /* background-image: url(""); */
}

.border{
  width:96%;
  height:96%;
  border: 1px solid white;
  position:relative
}

.img_container{
  width: 100%;
  height: 12rem;
  backdrop-filter: blur(5px) brightness(140%);
  position:absolute;
  bottom:0;
  display:flex;
  justify-content: space-around;
  align-items: center;
}

.img_container img{
  height: 85%;
  box-shadow: 0px 5px 10px 5px rgba(0,0,0,0.2);
}

</style>