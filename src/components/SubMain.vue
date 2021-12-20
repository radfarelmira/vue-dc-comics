<template>
    <section>
        <div class="products container">
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <img :src="link.imgSrc"  :alt="link.text">
                    <a href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: "Header",
    data: function () {
        return {
            links: [
                {
                    text: 'digital comics',
                    url: '#',
                    imgSrc: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    text: 'dc merchandise',
                    url: '#',
                    imgSrc: require('../assets/img/buy-comics-merchandise.png')
                },
                {
                    text: 'subscription',
                    url: '#',
                    imgSrc: require('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    text: 'comic shop locator',
                    url: '#',
                    imgSrc: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    text: 'dc power visa',
                    url: '#',
                    imgSrc: require('../assets/img/buy-dc-power-visa.svg')
                }     
            ]
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';
@import '../style/variables.scss';

section {
    background-color: $primary_color;
    color: $secondary_color;
    text-transform: uppercase;
    font-size: 14px;
    
    .products{
        padding: 40px 0;

        ul{
            display: flex;
            justify-content: space-around;

            li{
                display: flex;
                align-items: center;

                img{
                    width: 40px;
                }

                a{
                    color: inherit;
                    margin-left: 10px;
                    }
            }
        }
    }

}

</style>