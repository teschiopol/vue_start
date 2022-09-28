<script>
  export default {
    data() {
      return {
        count: 0,
        titleClass: 'title',
        text: ''
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
  <input v-model="text" placeholder="Type here">
  <p>{{ text }}</p>
</template>

<style scoped>
  button {
    font-weight: bold;
  }
  .title{
    color: lightskyblue;
  }
</style>
