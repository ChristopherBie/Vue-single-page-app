<template>
    <nav>
        <ul>
            <li><a id="home" href='#'>Home</a></li>
            <li><a href='#'>Locations and hours</a></li>
            <li><a href='#'>About us</a></li>
            <li><a href='#'>Reviews</a></li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'VueMenu'
}
</script>

<style scoped>
    ul, li {
        display: inline;
        padding: 30px;
        padding-top: 100px;
        margin-top: 100px;
    }
</style>