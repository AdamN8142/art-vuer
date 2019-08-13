<template>
  <div class="container">
    <div v-bind:key="image.id" v-for="image in images">
      <Card v-bind:image="image"/>
    </div>
  </div>
</template>


<script>
  import Card from './Card'

  export default {
    name: 'CardContainer',
    props: ['images'],
    components: {
      Card
    }
  }
</script>



<style scoped>

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 140px;

}


</style>
