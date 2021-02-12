<template>
    <div class="header">
        <div class="container">
            <div class="logo">Sezo vue</div>
            <div id="nav" class="text-right">
                <router-link to="/">Home</router-link>
                <router-link to="/blog">Blog</router-link>
                <router-link to="/about">About</router-link>
                <router-link to="/help">Help</router-link>
                <!-- 
                    replace if user click back then he will be directed back to home
                    exact give active class to excat link 
                -->
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "AppHeader"
};
</script>
<style lang="scss" scoped>
.header {
    background-color: #333;
    color: #fff;
    overflow: hidden;
    .logo {
        font-size: 30px;
        padding: 20px;
        float: left;
        width: 200px;
    }
    #nav {
        width: calc(100%-200px);
        a {
            padding: 20px;
            color: #fff;
            text-decoration: none;
        }
    }
}
</style>
