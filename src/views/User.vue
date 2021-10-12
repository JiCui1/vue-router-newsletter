<template>
  <div class="container" >
    <div class="border">
        <div class="user_info">
          <h1>Salutation: {{$route.params.salut}}</h1>
          <h1>First Name: {{$route.params.first}}</h1>
          <h1>Last Name: {{$route.params.last}}</h1>
          <h1>Age: {{$route.params.age}}</h1>
          <h1>Country: {{$route.params.country}}</h1>
        </div>
    </div>
  </div>
</template>

<script>
// import TextComp from '../components/TextComp.vue'

// export default {
//   name: 'Game',
//   components: {
//     TextComp
//   }
// }
</script>


<style scoped>
.container{
  width:100%;
  height: 100vh;
  background-color:#1f003eca;
  color:white;
  text-align: left;
  display:flex;
  justify-content: center;
  align-items: center;
}

.border{
  width: 96%;
  height: 96%;
  border: 2px solid white;
  display:flex;
  justify-content: center;
  align-items: center;
}

.user_info{
  color:#1f003eca;
  background-color:white;
  width: 25rem;
  height: 35rem;
  border-radius: 30px;
  padding:2rem;
  box-shadow: 0px 5px 15px 5px #000000;
  font-size:1rem;
}
</style>
