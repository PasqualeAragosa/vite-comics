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
        <div class="wrapper">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <!-- /.logo -->
            <nav class="navbar">
                <a v-for="item in menu" :class="item.text === 'Comics' ? 'active' : ''" :href="item.href">
                    {{ item.text }}
                </a>
            </nav>
            <!-- /.navbar -->
        </div>
        <!-- /.wrapper -->
    </header>
</template>
<style>

</style>