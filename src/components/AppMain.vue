<script>
import ProductList from './AppMain/ProductList.vue';
import ShowCase from './AppMain/ShowCase.vue';

export default {
    name: 'AppMain',
    components: {
        ProductList,
        ShowCase
    }
}
</script>

<template>
    <main>
        <ProductList></ProductList>
        <ShowCase></ShowCase>
    </main>
</template>

<style lang="scss" scoped>

</style>