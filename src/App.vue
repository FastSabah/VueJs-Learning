<template>
<img alt="Vue logo" src="./assets/logo.png">
<h1> This is App.Vue Code</h1>
<HomeF />
</template>

<script>
import HomeF from './components/Home.vue'

export default {
    name: 'App',
    components: {
        HomeF
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
