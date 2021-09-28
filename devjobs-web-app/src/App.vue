<template>
  <div id="app">
    <Header/>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  text-align: center;
  background-color: $lightGrey;
}

</style>

<script>
import Header from './components/Header.vue'

export default {

components:{
  Header
}
}
</script>
