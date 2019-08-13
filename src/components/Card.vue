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

<style scoped>
.image {
  height:500px;
  width: 700px;
}
.card {
  padding:20px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.image-date{
  font-size: 50px;
  font-family: cursive;
}

</style>
