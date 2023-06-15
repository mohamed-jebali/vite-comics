<template lang="">
    <div class='container-header mg-auto'>     
        <header class="flex">
            <div class='brand'>
                <img src="../../public/img/dc-logo.png" alt="dc-logo">
            </div>
            <nav class='navbar-header'>
                <ul class='flex'>
                    <li v-for="liElements in headerList">{{liElements}}</li>
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


.container-header{
    max-width: 1200px;
}

header{
    @include flex(row,space-between);
}

ul{
    li{
        @include flex();
        color : $DcNavColor;
        margin-right: 1rem;
    }
}

</style>