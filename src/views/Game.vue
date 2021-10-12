<template>
  <div class="game" >

    <div  v-if="$route.params.name=='darq'" class="bg" :style="{'background-image': 'url(' + require('../assets/darq.jpg') + ')'}">
      <div class="border">
        <TextComp titleText="Darq" description="DARQ tells the story of Lloyd, a boy who finds himself in the
        middle of a lucid nightmare. Unable to wake up, Lloyd 
        has to face his fears and decipher the meaning of the dream."/>
      </div>
    </div>

    <div  v-else-if="$route.params.name=='hollow'" class="bg" :style="{'background-image': 'url(' + require('../assets/hollow.jpg') + ')'}">
      <div class="border">
        <TextComp titleText="Hollow Knight" description="Forge your own path in Hollow Knight! An epic 
        action adventure through a vast ruined kingdom of 
        insects and heroes. Explore twisting caverns, 
        battle tainted creatures and befriend bizarre bugs, 
        all in a classic, hand-drawn 2D style."/>
      </div>
    </div>

    <div  v-else-if="$route.params.name=='dyson'" class="bg" :style="{'background-image': 'url(' + require('../assets/dyson.jpg') + ')'}">
      <div class="border">
        <TextComp titleText="Dyson Sphere" description="Dyson Sphere Program is a factory simulation game 
developed by Youthcat Studio released for Microsoft
 Windows in January 2021 in early access."/>
      </div>
    </div>

    <h1 v-else>Game no exist</h1>
  </div>
</template>

<script>
import TextComp from '../components/TextComp.vue'

export default {
  name: 'Game',
  components: {
    TextComp
  }
}
</script>


<style scoped>
  .bg{
    width: 100%;
    height: 100vh;
    background-size:cover;
    display:flex;
    justify-content: center;
    align-items: center;
  }

  .border{
    width:96%;
    height: 96%;
    border: 2px solid white;
  }
</style>
