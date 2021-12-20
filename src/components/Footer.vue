<template>
    <footer>
        <div class="top">
            <div class="content container">
                <div class="links">
                    <div class="link">
                        <h3>Title</h3>
                        <ul>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li> 
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li> 
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li> 
                        </ul>
                    </div>

                    <div class="link">
                        <h3>Title</h3>
                        <ul>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li> 
                        </ul>
                    </div>

                    <div class="link">
                        <h3>Title</h3>
                        <ul>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                            <li>
                                <a href="#">link</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="bottom">
            <div class="content container">
                <div class="bottom-left">
                    <a class="btn" href="#">
                    sign-up now!
                    </a>
                </div>

                <div class="bottom-right">
                    <a href="#">follow us</a>
                    <a href="#">
                        <img src="../assets/img/footer-facebook.png" alt="facebook">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-twitter.png" alt="twitter">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-youtube.png" alt="youtube">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-periscope.png" alt="periscope">
                    </a>
                </div>
                
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>
@import '../style/common.scss';
@import '../style/variables.scss';
 footer{
     background-image: url(../assets/img/footer-bg.jpg);
    .top{ 
        .content{
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-position: right;
            padding: 50px 0;
            display: flex;

            .links{
                display: flex;
                .link{
                    margin-right: 50px;
                    h3{
                        color: $secondary-color;
                    }

                    ul{
                        margin: 10px 0;
                        li{
                            margin: 5px 0;
                            a{
                              color: rgb(112, 111, 111);
                            }
                        }
                    }
                }
            }
        }
    }

    .bottom{
        background-color: #303030;
        padding: 30px 0;
        text-transform: uppercase;

        .content{
            display: flex;
            justify-content: space-between;
            align-items: center;
            .bottom-left{
                .btn{
                padding: 15px 10px;
                color: $secondary_color;
                border: 2px solid $primary_color;
                }
            }

            .bottom-right{
                display: flex;
                align-items: center;

                img{
                    margin-left: 20px;
                }

                a{
                    font-size: 20px;
                    font-weight: bold;
                    color: $primary_color;
                }
            }
        }
        
    }
 }

</style>