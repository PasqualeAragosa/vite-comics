<script>
export default {
    name: 'SiteMain',
    data() {
        return {
            list: [
                {
                    text: 'Digital Comics',
                    src: '../assets/img/buy-comics-digital-comics.png',
                },
                {
                    text: 'DC Merchandise',
                    src: '../assets/img/buy-comics-merchandise.png',
                },
                {
                    text: 'Subscription',
                    src: '../assets/img/buy-comics-subscription.png',
                },
                {
                    text: 'Comics Shop Locator',
                    src: '../assets/img/buy-comics-shop-locator.png',
                },
                {
                    text: 'DC Power Visa',
                    src: '../assets/img/buy-comics-power-visa.png',
                },
            ]
        }
    }
}
</script>

<template>
    <main id="site-main">
        <div class="content">
            <div class="wrapper"></div>
            <!-- /.wrapper -->
        </div>
        <!-- /.content -->
        <div class="digital-comix">
            <div class="wrapper">
                <ul>
                    <li v-for="item in list" class="">
                        <img :src="item.src" alt="">
                        {{ item.text }}
                    </li>
                </ul>
            </div>
            <!-- /.wrapper -->
        </div>
        <!-- /.digital-comix -->
        <div class="info-box">
            <div class="wrapper"></div>
            <!-- /.wrapper -->
        </div>
        <!-- /.info-box -->
    </main>
    <!-- /#site-main -->
</template>
<style>

</style>