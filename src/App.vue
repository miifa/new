<!-- App.vue -->
<template>
<div id="app">
    <ul>
        <li><router-link to="/" exact>Home</router-link></li>
        <li><router-link to="/products">Products</router-link></li>
    </ul>
    <router-view :data="myData"></router-view>
</template>

<script>
import CompHoge from './components/CompHoge'
import myData from '../static/data.json'

export default {
  components: {
    CompHoge 
  },
  data () {
    return {
      myData: myData
    }
  }
}
</script>