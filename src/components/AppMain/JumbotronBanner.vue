<script>
export default {
    name: 'JumbotronBanner'
}
</script>

<template>
    <div class="jumbotron">
        <img src="../../assets/img/jumbotron.jpg" alt="">
    </div>
    <!-- /.jumbotron -->
</template>

<style lang="scss">
.jumbotron {
    height: 350px;

    img {
        width: 100%;
        height: 350px;
        object-fit: cover;
        object-position: top;

    }
}
</style>