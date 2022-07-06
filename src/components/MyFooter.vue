<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="footer-list">
                    <div>
                        <ul>
                            <li class="first-li">DC COMICS</li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>

                         <ul>
                            <li class="first-li">SHOP</li>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>

                    <ul>
                        <li class="first-li">DC</li>
                        <li>Terms of Use</li>
                        <li>Privacy policy(New)</li>
                        <li>Ad Choices</li>
                        <li>Advertisings</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>

                    <ul>
                        <li class="first-li">SITES</li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>

                    
                </div>
                <div class="footer-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="logo">
                </div>
            </div>
        </div>

        <div class="footer-bottom">
            <div class="container">
                <div class="sign">
                    <div>SIGN-UP NOW!</div>
                </div>

                <div class="socials">
                    <ul>
                        <li class="follow">FOLLOW US</li>
                        <li>
                            <img src="../assets/img/footer-facebook.png" alt="socials">
                        </li>
                        <li>
                            <img src="../assets/img/footer-twitter.png" alt="socials">
                        </li>
                        <li>
                            <img src="../assets/img/footer-youtube.png" alt="socials">
                        </li>
                        <li>
                            <img src="../assets/img/footer-periscope.png" alt="socials">
                        </li>
                        <li>
                            <img src="../assets/img/footer-pinterest.png" alt="socials">
                        </li>

                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter'
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    footer {
        .footer-top{
            background-image: url('../assets/img/footer-bg.jpg');
            height: 300px;
            overflow: hidden;

            .footer-list {
                padding-top: 20px;
                padding-bottom: 30px;
                display: flex;

                ul {
                    margin-right: 30px;

                    li {
                        font-size: 10px;
                        margin: 5px 0;
                        color: lightgray;

                        &.first-li {
                            font-size: 16px;
                            font-weight: 600;
                            margin: 15px 0;
                            color: $secondary_color;
                        }
                    }
                }
            }
            .footer-logo {
                img {
                    width: 500px;
                }
            }
        }
        .footer-bottom {
            height: 100px;
            background-color: #303030;

            .sign {
                div {
                    color: $secondary_color;
                    background-color: #303030;
                    border: 2px solid $primary_color;
                    padding: 10px;
                }
            }
            .socials {

                ul {
                    display: flex;
                    align-items: center;
    
                    li {
                        margin: 10px;

                        &.follow {
                            color: $primary_color;
                            font-weight: 600;
                        }
                    }
                }
            }
        }
    }
</style>