<!-- Home.vue -->
<template>
  <span>{{data}}</span>
  <comp-hoge :data="data"><comp-hoge>
</template>

<script>
import CompHoge from '../components/CompHoge'
export default {
  components: {
    CompHoge
  },
  props: ['data']
}
</script>