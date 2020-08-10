<template>
    <div id="app">
        {{n}}
        <button @click="add">+1</button>
        <button @click="minus">-1</button>
        <button @click="zero">清零</button>
    </div>
</template>

<script>


  export default {
    name: 'App',
    // data是函数，medthods是对象。
    data() {
      return {
        n: 0
      }
    },
    methods: {
      add() {
        this.n += 1
      },
      minus(){
        this.n -=1
      },
      zero(){
        if (this.n===0){
          alert('当前已经清零！')
        }
        this.n =0
      }
    }
  }
</script>

<style lang="scss">
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
