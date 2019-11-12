<template>
  <div id="app">
    <vis-navbar></vis-navbar>
    <vis-sidebar></vis-sidebar>
    <vis-content v-html="test_html"></vis-content>

    <input type=text @input="test_html = $event.target.value">
  </div>
</template>

<script>


export default {
    name: 'app',
    data(){
        return {
            test_html:"<h1> Hello world </h1>"
        }
    }
}
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
