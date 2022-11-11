<script>
import InfoBox from './AppFooter/InfoBox.vue';

export default {
    name: 'AppFooter',
    components: {
        InfoBox
    }
}
</script>

<template>
    <footer>
        <InfoBox></InfoBox>
        <div class="footer-bottom">
            <div class="container">
                <div class="register">
                    <span>Sign Up Now!</span>
                </div>
                <!-- /.register -->
                <div class="social">
                    <span>Follow us</span>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                </div>
                <!-- /.social -->
            </div>
            <!-- /.container -->
        </div>
        <!-- /.footer-bottom -->
    </footer>
</template>

<style lang="scss" scoped>
.footer-bottom {
    background-color: #1C1C1C;

    .container {
        height: 100px;
        max-width: 1100px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .register {
            span {
                display: inline-block;
                text-transform: uppercase;
                padding: 0.5rem 0.75rem;
                border: 4px solid #0282f9;

                &:hover {
                    background-color: #0282f9;
                }
            }
        }

        .social {
            display: flex;
            align-items: center;

            span {
                margin-right: 2rem;
                text-transform: uppercase;
                font-size: 1.5rem;
                color: #0282f9;
            }

            img {
                padding: 0.5rem;
            }
        }
    }
}
</style>