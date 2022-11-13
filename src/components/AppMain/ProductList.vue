<script>
import ProductItem from './ProductItem.vue';
import dc_comics from '../../data/dc_comics.js';

export default {
    name: 'ProductList',
    components: {
        ProductItem
    },
    data() {
        return {
            products: dc_comics
        }
    }
}
</script>

<template>
    <div class="container_list">
        <span class="current">Current Series</span>
        <div class="row">
            <div class="col-2" v-for="product in products">
                <ProductItem :image="product.thumb" :title="product.series"></ProductItem>
            </div>
            <!-- /.col-2 -->
            <span>Load More</span>
        </div>
        <!-- /.row -->
    </div>
    <!-- /.container -->
</template>

<style lang="scss">
.container_list {
    max-width: 1100px;
    margin: auto;
    padding: 1.5rem 1rem 2.5rem 1rem;
    position: relative;

    span.current {
        text-transform: uppercase;
        background-color: #0282f9;
        padding: 0.5rem 1rem;
        font-size: 1.5rem;
        position: absolute;
        top: -5%;
        left: -1%;
    }

    .row {
        display: flex;
        flex-wrap: wrap;

        .col-2 {
            width: calc((100% / 12) * 2);
        }

        span {
            text-transform: uppercase;
            background-color: #0282f9;
            margin: auto;
            font-size: 1rem;
            padding: 0.5rem 2.5rem;
            position: static;
        }
    }

}
</style>