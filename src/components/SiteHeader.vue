<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            menu: [
                {
                    text: 'Characters',
                    href: '#'
                },
                {
                    text: 'Comics',
                    href: '#'
                },
                {
                    text: 'Movies',
                    href: '#'
                },
                {
                    text: 'Tv',
                    href: '#'
                },
                {
                    text: 'Games',
                    href: '#'
                },
                {
                    text: 'Collectibles',
                    href: '#'
                },
                {
                    text: 'Videos',
                    href: '#'
                },
                {
                    text: 'Fans',
                    href: '#'
                },
                {
                    text: 'News',
                    href: '#'
                },
                {
                    text: 'Shop',
                    href: '#'
                },

            ]
        }
    }
}
</script>

<template>
    <header id="site-header">
        <div class="logo">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
        <!-- /.logo -->
        <nav class="navbar">
            <a v-for="item in menu" :class="item.text === 'Comics' ? 'active' : ''" :href="item.href">
                {{ item.text }}
            </a>
        </nav>
        <!-- /.navbar -->
    </header>
</template>
<style>

</style>