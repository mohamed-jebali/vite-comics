<template>
    <div class='container-footer-top'>     
        <footer class="mg-auto flex">
            <div class="list-wrapper flex">
                <nav class='list-footer'>
                    <h2>
                        DC COMICS
                    </h2>
                    <ul>
                        <li v-for="liElements in headerList">{{liElements}}</li>
                    </ul>
                    <h2>
                        SHOPS
                    </h2>
                    <ul>
                        <li>
                            <li>Shop DC</li>
                        <li>Shop Collectibles</li>
                        </li>
                    </ul>
                </nav>
                <nav class='list-footer'>
                    <h2>
                        DC
                    </h2>
                    <ul>
                        <li v-for="liElements in headerList">{{liElements}}</li>
                    </ul>
                </nav>
                <nav class='list-footer'>
                    <h2>
                        SITES
                    </h2>
                    <ul>
                        <li v-for="liElements in headerList">{{liElements}}</li>
                    </ul>
                </nav>
            </div>
            <div class='brand'>
                <!-- <img src="../../public/img/dc-logo-bg.png" alt="dc-logo-background"> -->
            </div>
        </footer>
    </div>
</template>
<script>
import { createApp } from 'vue'
export default{
    data(){
        return{
            headerList:["CHARACTERS","COMICS","MOVIES","TV","GAMES",,"COLLECTIBLES","VIDEOS","FANS","NEWS","SHOP"]
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
    z-index: 0;
    background-image: url(/public/img/dc-logo-bg.png);
    background-size: contain;
    height: 450px;
    width: 50%;
    background-repeat: no-repeat;
}

.list-wrapper{
    padding-top: 3rem;
}
.list-footer{
    margin-right: 2rem;
}

.container-footer-top{
    background-image: url(../../public/img/footer-bg.jpg);
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