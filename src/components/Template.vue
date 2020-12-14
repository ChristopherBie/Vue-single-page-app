// FileName.vue

<template>
    <h3>I am the [file name] component</h3>
</template>

<script>
    export default {
        name: 'VueFileName' or "vue-file-name",  //does not have to be the same as in App.vue
    }
</script>

<style lang="scss" scoped>

</style>



// App.vue

<template>
    <div id="app">
        <vue-header></vue-header>
        <vue-menu></vue-menu>
        <vue-body></vue-body>
        <vue-side-bar></vue-side-bar>
        <vue-footer></vue-footer>
        <vue-file-name></vue-file-name>
    </div>
</template>

<script>
    import VueHeader from './components/Header.vue';
    import VueMenu from './components/Menu.vue';
    import VueBody from './components/Body.vue';
    import VueSideBar from './components/SideBar.vue';
    import VueFooter from './components/Footer.vue';
    import VueFileName from './components/FileName.vue';

    export default {
        name: 'App',
        components: {
            VueHeader,
            VueMenu,
            VueBody,
            VueSideBar,
            VueFooter,
            VueFileName, //comma here too?
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


