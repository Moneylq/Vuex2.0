<template>
  <div id="app">
    Count is {{ $store.state.count }}
    <button @click="increment">+5</button>
    <button @click="decrement">-3</button>
  </div>
</template>
<script>
  import { mapGetters,mapActions } from 'vuex'
  export default {
    computed: mapGetters([
      ]),
    methods: mapActions([
      'increment',
      'decrement'
      ])
  }
</script>