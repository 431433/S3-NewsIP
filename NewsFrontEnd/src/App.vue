<template>
    <div id="app">
        <Home msg="Hello world!" />
    </div>
</template>

<script lang="ts">
    import { Component, Vue } from 'vue-property-decorator';
    import Home from './components/Home.vue';
    import NavBar from './components/NavBar.vue';

    @Component({
        components: {
            Home,
            NavBar
        }
    })
    export default class App extends Vue { }
</script>

<style>
</style>
