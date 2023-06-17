<template lang="">
    <div class='container mg-auto'>     
        <header class="flex">
            <div class='brand'>
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
            </div>
                <ul class='flex'>
                    <li v-for="liElements,index in headerList" :class="liElements.active === true ? 'activeColor' : ''" @click='toggleActive(index)'>
                        {{liElements.text}}
                    </li>
                </ul>
        </header>
    </div>
</template>
<script>
import { createApp } from 'vue'
export default{
    data(){
        return{
            headerList:[
                {
                    text:"CHARACTERS",
                    active: false
                },
                {
                    text:"COMICS",
                    active: true,
                },
                {
                    text:"MOVIES",
                    active: false,
                },
                {
                    text:"TV",
                    active: false,
                },
                {
                    text:"GAMES",
                    active: false,
                },
                {
                    text:"COLLECTIBLES",
                    active: false,
                },
                {
                    text:"VIDEOS",
                    active: false,
                },
                {
                    text:"FANS",
                    active: false,
                },
                {
                    text:"NEWS",
                    active: false,
                },
                {
                    text:"SHOP",
                    active: false,
                },
            ],

        }
    },
    methods: {
    toggleActive(index) {
      this.headerList.forEach((item, i) => {
        item.active = i === index;
      });
    }
  }
}

</script>
<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;


.container{
    max-width: 1000px;
}

.brand{

    img{
        height: 60px
    }
}

header{
    @include flex(row,space-between);
    height: 90px;
}


ul{
    height: 100%;
    li{
        @include flex();
        color : $DcNavColor;
        margin-right: 1.5rem;
        font-size: 0.65rem;
        font-weight: 600;
        height: 100%;

        &:hover{
            text-decoration: underline;
        }
    }
    li:nth-child(2){
            color: $DcColorBlue;
        }
        .activeColor{
            border-bottom: 4px solid $DcColorBlue ;
        }
}

</style>