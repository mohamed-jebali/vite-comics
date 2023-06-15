<template>
    <div class='container-footer-top'>     
        <footer class="mg-auto">
            <nav class='list-footer'>
                <h2>
                    DC COMICS
                </h2>
                <ul>
                    <li v-for="liElements in headerList">{{liElements}}</li>
                </ul>
            </nav>
            <div class='brand'>
                <img src="../../public/img/dc-logo-bg.png" alt="dc-logo">
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
}

.brand{
    img{
        width: 70%;
    }
}

.container-footer-top{
    background-image: url(../../public/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: contain;
    height: 600px;
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
        font-size: 0.65rem;
        font-weight: 600;
        margin-bottom: 0.5rem;

        &:hover{
            text-decoration: underline;
        }
    }
}

</style>