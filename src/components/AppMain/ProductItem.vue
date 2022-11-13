<script>
export default {
    name: 'ProductItem',
    props: {
        image: String,
        price: String,
        title: String,
        type: String
    }
}
</script>

<template>
    <div class="card">
        <div class="product">
            <img :src="image" alt="">
            <h4>{{ title }}</h4>
        </div>
        <!-- /.product -->
    </div>
    <!-- /.card -->
</template>

<style lang="scss">
.card {
    padding: 0.75rem 0;

    img {
        width: 150px;
        aspect-ratio: 1 / 1;
        object-fit: cover;
        object-position: top;
    }

    h4 {
        text-transform: uppercase;
    }
}
</style>