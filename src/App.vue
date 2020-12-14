<template>
    <div id="app">
        <vue-header id="header"></vue-header>
        <vue-menu id="menu"></vue-menu>
        <vue-body id="body"></vue-body>
        <vue-sidebar id="sidebar"></vue-sidebar>
        <vue-meet-the-team id="meet-the-team"></vue-meet-the-team>
        <vue-footer id="footer"></vue-footer>
    </div>
</template>

<script>
    import VueHeader from './components/Header.vue';
    import VueMenu from './components/Menu.vue';
    import VueBody from './components/Body.vue';
    import VueSidebar from './components/Sidebar.vue';
    import VueMeetTheTeam from './components/MeetTheTeam.vue';
    import VueFooter from './components/Footer.vue';

    export default {
        name: 'App',
        components: {
            VueHeader,
            VueMenu,
            VueBody,
            VueSidebar,
            VueMeetTheTeam,
            VueFooter
        }
    }
</script>

<style>
    #app {
        box-sizing: border-box;
        margin: 0px;
        padding: 0px;
        min-height: 100vh;
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: black;
        display: grid;
        grid-template-rows: 100px 22px 3fr 2fr 100px;
        grid-template-columns: 1fr 5fr;
        grid-template-areas:
            'header header'
            'menu-bar menu-bar'
            'sidebar body'
            'sidebar meettheteam'
            'footer footer';
    }
    #header {
        grid-area: header;
        background-color: blue;
        color: white;
    }
    #menu {
        grid-area: menu-bar;
        background-color: skyblue;
        padding-left: 5px;
    }
    #body {
        grid-area: body;
        background-color: red;
    }
    #sidebar {
        grid-area: sidebar;
        background-color: yellow;
    }
    #meet-the-team {
        grid-area: meettheteam;
        background-color: green;
    }
    #footer {
        grid-area: footer;
        background-color: blue;
        color: white;
    }
</style>
