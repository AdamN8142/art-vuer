<template>
  <div class="container">
    <Card />
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


</style>
