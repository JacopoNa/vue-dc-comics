<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="dc logo">
            </div>

            <div class="menu">
                <ul>
                    <li v-for="(element,index) in menuList" :key="index" :class="{ 'current' : element.status === true}">
                        {{ element.text }}
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'MainHeader',
    data() {
        return {
            menuList: [
            {
                text: 'CHARACTERS',
                status: false
            },
            {
                text: 'COMICS',
                status: true
            },
             {
                text: 'MOVIES',
                status: false
            },
             {
                text: 'TV',
                status: false
            },
             {
                text: 'GAMES',
                status: false
            },
             {
                text: 'COLLECTIBLES',
                status: false
            },
             {
                text: 'VIDEOS',
                status: false
            },
             {
                text: 'FANS',
                status: false
            },
             {
                text: 'NEWS',
                status: false
            },
             {
                text: 'SHOP',
                status: false
            }
        ]
        }
        
    }
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