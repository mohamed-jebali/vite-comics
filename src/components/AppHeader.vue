<template lang="">
    <div class='container-header mg-auto'>     
        <header class="flex">
            <div class='brand'>
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
            </div>
            <nav class='navbar-header'>
                <ul class='flex'>
                    <li v-for="liElements in headerList">
                        {{liElements}}
                    </li>
                </ul>
            </nav>
        </header>
    </div>
</template>
<script>
import { createApp } from 'vue'
export default{
    data(){
        return{
            headerList:["CHARACTERS","COMICS","MOVIES","TV","GAMES","COLLECTIBLES","VIDEOS","FANS","NEWS","SHOP"]
        }
    },
    methods:{

    }
}

</script>
<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;


.container-header{
    max-width: 1000px;
}

header{
    @include flex(row,space-between);
    margin: 1rem 0;
}


ul{
    li{
        @include flex();
        color : $DcNavColor;
        margin-right: 1.5rem;
        font-size: 0.65rem;
        font-weight: 600;

        &:hover{
            text-decoration: underline;
        }
    }
    li:nth-child(2){
            color: $DcColorBlue;
        }
}

</style>