<template>
    <div id="app">
        {{library}}
        <img src="./assets/logo.png">
        <hello></hello>
    </div>
</template>

<script>
import Hello from './components/Hello'
import Library from './data/TranslationRepo.js'

export default {
    name: 'app',
    components: {
        Hello
    },
    data: () => {
        return {
            library: Library.lexicon
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
