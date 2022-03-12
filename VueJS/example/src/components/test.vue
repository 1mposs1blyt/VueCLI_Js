<template>
  <main>
      <h1 v-bind:class="{color: color}">hello</h1>
      <button v-on:click="func">Click!</button>
      <h2>{{count}}</h2>
      <p>{{name}}</p>
  </main>
</template>

<script>
export default {
  name: "TestComponent",
  namesurname:{
      name:"Vasya",
      surname:"Ivanov"
  },
  data(){
      return{
          count: 1,
          color: false
      }
  },
  methods:{
      func (){
          this.count++
        //   alert("clicked!");// v-on:mouseover="func" v-on:mouseout="func"
      },watch:{
          count: function(){
            this.color != this.color
          },
      }
  },
};
</script>

<style lang="less">
.color{
    background: rgb(255, 0, 0);
}
</style>