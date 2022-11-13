<script>
import JumbotronBanner from './AppMain/JumbotronBanner.vue'
import ProductList from './AppMain/ProductList.vue';
import ShowCase from './AppMain/ShowCase.vue';

export default {
    name: 'AppMain',
    components: {
        JumbotronBanner,
        ProductList,
        ShowCase,
    }
}
</script>

<template>
    <main>
        <JumbotronBanner></JumbotronBanner>
        <ProductList></ProductList>
        <ShowCase></ShowCase>
    </main>
</template>

<style lang="scss" scoped>

</style>