<template>
  <div id="app">
    <router-wrapper></router-wrapper>
  </div>
</template>

<style>

</style>
<script>
import RouterWrapper from "./views/RouterWrapper";
export default {

  name: 'App',
  components: {
    'router-wrapper': RouterWrapper
  }
}
</script>
