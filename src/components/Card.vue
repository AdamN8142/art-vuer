<template>
  <div class="card">
    <img v-bind:src="image.baseimageurl"/>
  </div>
</template>

<script>
  export default {
    name: 'Card',
    props: ['image']
  }
</script>

<style scoped>


</style>
