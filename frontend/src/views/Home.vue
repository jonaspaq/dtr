<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/images/gifvue.gif">
    <HelloWorld msg="Welcome to DTR"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss" scoped>
.home {
  img {
    height: 200px;
    width: 400px;
  }
}
</style>
