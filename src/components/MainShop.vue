<template>
    <section class="shop">
        <div class="container">
            <ul>
                <li>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="dc image">
                    <span>DIGITAL COMICS</span>
                </li>

                 <li>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="dc image">
                    <span>DC MERCHANDISE</span>
                </li>

                 <li>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="dc image">
                    <span>SUBSCRIPTION</span>
                </li>

                 <li>
                    <img class="locator" src="../assets/img/buy-comics-shop-locator.png" alt="dc image">
                    <span>COMIC SHOP LOCATOR</span>
                </li>

                 <li>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="dc image">
                    <span>DC POWER VISA</span>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MainShop'
}
</script>

<style lang="scss" scoped>
    @import '../style/variables';

    .shop {
        background-color: $primary_color;
        padding: 40px 0;
        color: $secondary_color;

        .container {

            ul{
                width: 100%;
                display: flex;
                justify-content: space-around;
                align-items: center;
                li{

                    img{
                        width: 40px;
                        vertical-align: middle;
                        margin-right: 10px;
                        &.locator {
                            width: 30px;
                        }
                    }
                    span{
                        font-size: 12px;
                        vertical-align: middle;
                    }
                }
            }
        }
    }
</style>