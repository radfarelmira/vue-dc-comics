<template>
    <header class="container">
        <nav>
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="dc logo">
            </div>
        
        
            <div class="menu">
                <ul>
                    <li v-for="(link, index) in links" :key="index" :class="{current: link.current}">
                        <a href="link.url">{{link.text}}</a>
                    </li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function () {
        return {
            links: [
                {
                    text: 'characters',
                    url: '#',
                    current: true
                },
                {
                    text: 'comics',
                    url: '#',
                    current: false
                },
                {
                    text: 'movies',
                    url: '#',
                    current: false
                },
                {
                    text: 'tv',
                    url: '#',
                    current: false
                },
                {
                    text: 'games',
                    url: '#',
                    current: false
                },
                {
                    text: 'collectibles',
                    url: '#',
                    current: false
                },
                {
                    text: 'videos',
                    url: '#',
                    current: false
                },
                {
                    text: 'fans',
                    url: '#',
                    current: false
                },
                {
                    text: 'news',
                    url: '#',
                    current: false
                },
                {
                    text: 'shop',
                    url: '#',
                    current: false
                },
                
            ]
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';
@import '../style/variables.scss';

header{
    width: 100%;
    height: 104px;
    text-transform: uppercase;
    font-size: 14px;
    font-weight: bold;

    nav{
        width: 100%;
        height: 100%;
        display: flex;
        .logo{
            display: flex;
            align-items: center;

            img{
                width: 70px;
            }
        }

        .menu{
            text-align: right;
            flex-grow: 1;
            li{
                display: inline-block;
                line-height: 100px;
                margin-left: 20px;

                &.current{
                    color: $primary_color;
                    border-bottom: 5px solid $primary_color;
                }

                a{
                    text-decoration: none;
                    display: inline-block;
                    color: inherit;
                }
            }
        }
    }
}

</style>