<template>
    <div id="main">
        <v-header showBackBtn="true" headTitle="hello world"></v-header>
        <!--<user-count></user-count>
        <div class="banner">
            <div class="swiper-container">
                <div class="swiper-wrapper">
                    <div class="swiper-slide">
                       <img src="../assets/image/bg2.jpg" alt="">
                    </div>
                    <div class="swiper-slide">
                       <img src="../assets/image/bg3.jpg" alt="">
                    </div>
                    <div class="swiper-slide">
                       <img src="../assets/image/bg1.jpg" alt="">
                    </div>
                </div>
                <div class="swiper-pagination"></div>
            </div>
        </div>    -->
        <v-menu></v-menu>
        <v-footer></v-footer>
    </div>
</template>

<script>
import vHeader from '../components/Header'
// import userCount from '../components/userCount'
import vFooter from '../components/Footer'
import vMenu from '../components/Menu'
// import '../static/lib/js/swiper.min.js'
// import '../static/lib/css/swiper.min.css'

export default {
    data() {
        return {

        }
    },
    components: {
        vHeader,vFooter,vMenu
    },
    mounted() {
    //初始化swiper
    // new Swiper('.swiper-container', {
    //     pagination: '.swiper-pagination',
    //     loop: true
    // });
    },
    methods: {
     
    }

}
</script>

<style scoped lang="scss">
    #dragitem{
        width:100px;
        height:100px;
        background-color:red;
        position:absolute;
        left:100px;
        top:200px;
    }
    #main {
        font-family: "Microsoft Yahei", 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
    }
    .banner {
        .swiper-container {
            width: 100%;
            height: calc(100vh - 60px);
            .swiper-slide img {
                width: 100%;
                height: 100%;
            }
        }
    }
    .main-nav ul {
        display: flex;
        width: 100%;
        flex-direction: row;
        flex-wrap:  wrap;
        justify-content: center;
        align-items: center;
        li {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 25%;
            height: 100px;
            border: 1px solid #C7000B;
            box-sizing: border-box;
            span {
                color: #c96;
            }
        }
    }
    .router-fade-enter-active, .router-fade-leave-active {
        transition: opacity .3s;
    }
    .router-fade-enter, .router-fade-leave-active {
        opacity: 0;
    }
</style>