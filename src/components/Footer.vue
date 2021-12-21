<template>
    <footer>
        <div class="top">
            <div class="content container">
                <div class="links">
                    <div class="link">
                        <h3>dc comics</h3>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>
                        </ul>

                        <h3>shop</h3>
                        <ul>
                            <li>
                                <a href="#">Shop DC </a>
                            </li>
                            <li>
                                <a href="#">Shop DC Collectibles</a>
                            </li>
                        </ul>
                    </div>

                    <div class="link">
                        <h3>dc</h3>
                        <ul>
                            <li>
                                <a href="#">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy policy(New)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choices</a>
                            </li>
                            <li>
                                <a href="#">Advertising</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subscriptions</a>
                            </li> 
                            <li>
                                <a href="#">Talent Workshops</a>
                            </li> 
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li> 
                            <li>
                                <a href="#">Ratings</a>
                            </li> 
                            <li>
                                <a href="#">Shop Help</a>
                            </li> 
                            <li>
                                <a href="#">Contact Us</a>
                            </li> 
                        </ul>
                    </div>

                    <div class="link">
                        <h3>sites</h3>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
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
     
    .top{ 
        background-image: url(../assets/img/footer-bg.jpg);
        .content{
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-position: right;
            padding: 50px 0;
            display: flex;

            .links{
                width: 50%;
                display: flex;
                .link{
                    margin-right: 50px;
                    h3{
                        color: $secondary-color;
                        text-transform: uppercase;
                    }

                    ul{
                        margin: 20px 0;
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
            align-items: center;
            justify-content: space-between;
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
                    padding-left: 20px ;
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