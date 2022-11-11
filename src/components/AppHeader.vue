<script>

export default {
    name: 'AppHeader',
    data() {
        return {
            menu: [
                {
                    text: 'Characters',
                    href: '#'
                },
                {
                    text: 'Comics',
                    href: '#'
                },
                {
                    text: 'Movies',
                    href: '#'
                },
                {
                    text: 'TV',
                    href: '#'
                },
                {
                    text: 'Games',
                    href: '#'
                },
                {
                    text: 'Collectibles',
                    href: '#'
                },
                {
                    text: 'Video',
                    href: '#'
                },
                {
                    text: 'Fans',
                    href: '#'
                },
                {
                    text: 'News',
                    href: '#'
                },
                {
                    text: 'Shop',
                    href: '#'
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <nav class="navbar">
            <div class="container">
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <!-- /.logo -->
                <ul class="main-menu">
                    <li v-for="item in menu">
                        <a :href="item.href"> {{ item.text }} </a>
                    </li>
                </ul>
                <!-- /.main-menu -->
            </div>
            <!-- /.container -->
        </nav>
        <!-- /.navbar -->
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header {
    background-color: white;

    .navbar {
        max-width: 1100px;
        margin: auto;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.25rem 0;

            .logo {
                img {
                    height: 100px;
                }
            }

            ul {
                list-style: none;
                display: flex;

                li {
                    a {
                        font-weight: 600;
                        margin: 0 1rem;
                        padding: 3.6rem 0;
                        text-transform: uppercase;
                        text-decoration: none;
                        color: grey;

                        &:hover {
                            color: #0282f9;
                            border-bottom: 5px solid #0282f9;
                        }
                    }
                }
            }
        }
    }
}
</style>