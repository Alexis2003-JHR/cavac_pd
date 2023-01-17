<template>
  <Loading/>
  <router-view/>
</template>

<script>
import Loading from "./components/Loading.vue"

export default{
  name: 'App',
  components: {Loading},
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=PT+Sans:ital,wght@0,400;0,700;1,400;1,700&display=swap');

*{
  font-family: 'PT Sans', sans-serif;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
</style>
