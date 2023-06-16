<template>
    <div class='container-footer-top'>     
        <footer class="mg-auto flex flex-nowrap">
            <div class="list-wrapper flex">
                <nav class='list-footer'>
                    <h2>
                        DC COMICS
                    </h2>
                    <ul>
                        <li v-for="liElements in dcComics">{{liElements}}</li>
                    </ul>
                    <h2>
                        SHOPS
                    </h2>
                    <ul>
                        <li v-for="liElements in shops">{{liElements}}</li>
                    </ul>
                </nav>
                <nav class='list-footer'>
                    <h2>
                        DC
                    </h2>
                    <ul>
                        <li v-for="liElements in dc">{{liElements}}</li>
                    </ul>
                </nav>
                <nav class='list-footer'>
                    <h2>
                        SITES
                    </h2>
                    <ul>
                        <li v-for="liElements in sites">{{liElements}}</li>
                    </ul>
                </nav>
            </div>
            <div class='brand'>

            </div>
        </footer>
    </div>
</template>
<script>
import { createApp } from 'vue'
export default{
    data(){
        return{
            dcComics:["CHARACTERS","COMICS","MOVIES","TV","GAMES","VIDEOS","FANS","NEWS"],
            dc:["Term of Use","Privacy policy (New)","Ad Choices","Advertising","Jobs","Subscription","Talent Workshops","CPSC Certificates","Ratings","Shop Help","Contact Us"],
            sites:["DC","MAD Magazine","Dc Kids","DC Universe","DC Power Visa"],
            shops:["Shop DC","Shop Collectibles"]
        }
    },
    methods:{

    }
}

</script>
<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;


h2{
    color: white;
    margin-bottom: 1.5rem;
}

.brand{
    position: relative;
    left: 55px;
    z-index: 1;
    background-image: url(/src/assets/img/dc-logo-bg.png);
    background-size: 534px;
    background-position: 27px;
    height: 427px;
    width: 57%;
    background-repeat: no-repeat;
}

.list-wrapper{
    padding-top: 3rem;
}
.list-footer{
    margin-right: 2rem;
}

.container-footer-top{
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

footer{
    max-width: 1000px;
    @include flex(row,space-between);
}

ul{
    li{
        @include flex(column,center,start);
        color : $DcFooterColorFont;
        margin-right: 1rem;
        font-size: 0.6rem;
        margin-bottom: 0.5rem;

        &:hover{
            text-decoration: underline;
        }
    }
}

</style>