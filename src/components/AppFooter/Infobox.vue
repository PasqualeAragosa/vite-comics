<script>
export default {
    name: 'InfoBox',
    data() {
        return {
            DcComics:
                [
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News'
                ],
            Shop:
                [
                    'shop DC',
                    'Shop DC Collectibles',
                ],
            Dc:
                [
                    'Term Of Use',
                    'Privacy policy (New)',
                    'Ad Choices',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Woekshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us',
                ],
            Sites:
                [
                    'DC',
                    'MAD Magazine',
                    'DC Kids',
                    'DC Universe',
                    'DC Power Visa',
                ],
        }
    }
}
</script>

<template>

    <div class="info-box">
        <div class="container">
            <div class="details">
                <div class="col">
                    <h4>DC Comics</h4>
                    <ul>
                        <li v-for="item in DcComics">{{ item }}</li>
                    </ul>
                    <h4>Shop</h4>
                    <ul>
                        <li v-for="item in Shop">{{ item }}</li>
                    </ul>
                </div>
                <!-- /.col -->
                <div class="col">
                    <h4>Dc</h4>
                    <ul>
                        <li v-for="item in Dc">{{ item }}</li>
                    </ul>
                </div>
                <!-- /.col -->
                <div class="col">
                    <h4>DC Comics</h4>
                    <ul>
                        <li v-for="item in Sites">{{ item }}</li>
                    </ul>
                </div>
                <!-- /.col -->
            </div>
            <!-- /.details -->
            <div class="logo">
                <!-- <img src="../../assets/img/dc-logo-bg.png" alt=""> -->
            </div>
            <!-- /.logo -->
        </div>
        <!-- /.container -->
    </div>
    <!-- /.info-box -->

</template>

<style lang="scss" scoped>
.info-box {
    background-image: url('../../assets/img/footer-bg.jpg');
    height: 400px;

    .container {
        max-width: 1100px;
        margin: 0 auto;
        color: rgb(191, 189, 189);
        display: flex;
        justify-content: space-between;

        .details {
            display: flex;
            flex-wrap: wrap;
            padding: 2rem 0;

            .col {
                width: calc((100% / 12) * 4);
                height: min-content;

                h4 {
                    text-transform: uppercase;
                    color: white;
                }

                ul {
                    list-style: none;
                    padding-top: 1rem;
                    margin-bottom: 2rem;
                    line-height: 1.5rem;
                    font-size: 14px;
                }

            }

        }

        .logo {
            height: 400px;
            width: 600px;
            background-image: url('../../assets/img/dc-logo-bg.png');
            background-size: 100%;
            background-repeat: no-repeat;
            background-position-y: center;
            background-position-x: left;
        }
    }
}
</style>