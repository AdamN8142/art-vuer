<template>
  <div id="app">
    <Header />

  </div>
</template>

<script>
import Header from './components/Header'
const url = "https://api.harvardartmuseums.org/image?apikey=688eb260-b190-11e9-95eb-6525f67b00a0"


export default {
  name: 'app',
  components: {
    Header
  },
  data() {
    return {
      images: [],
      errorMsg: ''
    }
  },
  mounted: function() {
    this.fetchImages()
  },

  methods: {
    fetchImages: function(){
      fetch(url)
        .then(result => result.json())
        .then(data => this.images = data.records)
        .catch(error => this.errorMsg = error)
    }
  }


}
</script>

<style>
* {
  box-sizing: border-box;
  margin:0;
  padding:0;
  background-color: rgba(28, 216, 191, 0.591);
}
</style>
