<template>
  <div>
    <BasicSetup />
    <p>{{ mytext }}</p>
  </div>
</template>
<script>
import { BasicSetup } from './components/BasicSetup.vue'

export default {
  components: {
        BasicSetup,
    },
    data () {
      return {
      mytext: "my text here!",
    };
  }
}
</script>

<style>

</style>

 <!-- <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view/> -->