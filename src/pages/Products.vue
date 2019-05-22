<!-- Products.vue -->
<template>
  <span>{{data}}</span>
  <comp-fuga :data="data"></comp-fuga>
</template>

<script>
import CompFuga from '../components/CompFuga'
export default {
  components: {
    CompFuga
  },
  props: ['data']
}
</script>