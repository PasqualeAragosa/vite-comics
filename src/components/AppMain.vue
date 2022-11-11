<script>
import ProductList from './AppMain/ProductList.vue';
import Showcase from './AppMain/Showcase.vue';

export default {
    name: 'AppMain',
    components: {
        ProductList,
        Showcase
    }
}
</script>

<template>
    <main>
        <ProductList />
        <Showcase />
    </main>
</template>

<style lang="scss" scoped>

</style>