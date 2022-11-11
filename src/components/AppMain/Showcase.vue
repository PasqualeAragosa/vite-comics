<script>
export default {
    name: 'ShowCase',
    data() {
        return {
            items: [
                {
                    icon: '/assets/img/buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    icon: '/assets/img/buy-comics-merchandise.png',
                    text: 'DC Merchandise'
                },
                {
                    icon: '/assets/img/buy-comics-shop-locator.png',
                    text: 'Subscriptions'
                },
                {
                    icon: '/assets/img/buy-comics-subscriptions.png',
                    text: 'Comic Shop Locator'
                },
                {
                    icon: '/assets/img/buy-dc-power-visa.svg',
                    text: 'Dc poer visa'
                }
            ]
        }
    }
}
</script>

<template>
    <div class="show-case">
        <div class="container">
            <div class="item" v-for="item in items">
                <img :src="'/src' + item.icon" alt="">
                <span>{{ item.text }}</span>
            </div>
            <!-- /.item -->
        </div>
        <!-- /.container -->
    </div>
    <!-- /.show-case -->
</template>

<style lang="scss" scoped>
.show-case {
    background-color: blue;

    .container {
        max-width: 1100px;
        margin: auto;
        display: flex;
        justify-content: space-evenly;
        padding: 1rem 0;

        .item {
            display: flex;
            align-items: center;
            text-transform: uppercase;
            font-size: 0.80rem;

            img {
                height: 50px;
                padding-right: 0.5rem;
            }
        }
    }
}
</style>