<template>
  <div class='card'>
    <p class="image-date">{{image.date}}</p>
    <img class="image" v-bind:src="image.baseimageurl"/>
  </div>
</template>

<script>
  export default {
    name: 'Card',
    props: ['image']
  }
</script>

<style>
.image {
  height:500px;
  width: 700px;
  border-radius: 10px;
}
.card {
  padding:20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: burlywood;
  width: 900px;
  border-radius: 20px;
  margin-bottom: 70px;
}
.image-date{
  font-size: 50px;
  font-family: cursive;
  background-color: wheat;
  color:brown;
  border-radius: 20px;
  margin-bottom: 20px;
}

</style>
