<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="dc logo">
            </div>

            <div class="menu">
                <ul>
                    <li>CHARACTERS</li>
                    <li class="current">COMICS</li>
                    <li>MOVIES</li>
                    <li>TV</li>
                    <li>GAMES</li>
                    <li>COLLECTIBLES</li>
                    <li>VIDEOS</li>
                    <li>FANS</li>
                    <li>NEWS</li>
                    <li>SHOP</li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'MainHeader'
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    header {
        height: 100px;
        font-size: 10px;
        font-weight: 600;

        .logo {
            img {
                width: 70px;
            }
        }

        .menu {

            ul {
                display: flex;
                li{
                    margin: 0 13px;
                    line-height: 100px;
                    
                    &.current {
                        color: $primary_color;
                        border-bottom: 3px solid $primary_color;
                    }
                }
            }
        }
    }
</style>