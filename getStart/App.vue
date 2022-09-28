<script>
  export default {
    data() {
      return {
        count: 0,
        titleClass: 'title'
      }
    },
    methods:{
      increment(){
        this.count++
      }
    }
  }
</script>

<template>
  <button @click="increment" v-bind:class="titleClass">Count is: {{ count }}</button>
</template>

<style scoped>
  button {
    font-weight: bold;
  }
  .title{
    color: lightskyblue;
  }
</style>
