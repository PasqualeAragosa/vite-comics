<script>
import ProductList from './AppMain/ProductList.vue';
import ShowCase from './AppMain/ShowCase.vue';
import JumbotronBanner from './AppMain/JumbotronBanner.vue'

export default {
    name: 'AppMain',
    components: {
        ProductList,
        ShowCase,
        JumbotronBanner
    }
}
</script>

<template>
    <main>
        <ProductList></ProductList>
        <ShowCase></ShowCase>
        <JumbotronBanner></JumbotronBanner>
    </main>
</template>

<style lang="scss" scoped>

</style>