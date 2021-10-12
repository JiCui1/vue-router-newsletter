<template>
    <div class="text_container">
        <div class="text_container">
            <h5>Special Deal</h5>
            <h1>{{titleText}} </h1>
            <p>{{description}}</p>
                <button>Order</button>
        </div>
      </div>
</template>

<script>
export default {
    name:"TextComp",
    props:{
        titleText: String,
        description: String,
    }
}
</script>

<style>
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
  width: 30rem;
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


</style>