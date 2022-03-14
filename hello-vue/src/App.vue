<template>
  <div>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
    </div>
    <router-view />

    <BasicSetup />
    <h1>{{ msg.toLocaleUpperCase() }}</h1>
    <p>{{ mytxt }}</p>
    <button v-on:click="logHello">Click to see</button>
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
        msg: "This is H1",
        mytxt: "txt from data",
    };
  },
  methods: {
    logHello(){
      alert('Hello World! from methods')
    }
  }
}
</script>

<style>
button {
  margin: 2rem;
  padding: 1.5rem;
  color: white;
  background-color: rgb(14, 138, 138);
}
</style>

 <!-- <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view/> -->