<template lang="">
    <div class='content-container'>
        <div class='title-content mg-auto'>
            <h1>
            BONUS
            </h1>
        </div>
    </div>
</template>
<script>
import { createApp } from 'vue'
export default{
    data(){
        return{

        }
    },
    methods:{

    }
}

</script>
<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;



div.content-container{
    color: white;
    background-color: $DcColorBlue;
    padding: 4rem;

    h1{
        text-align: center;
        font-size: 2rem;
    }
    .title-content{
        max-width: 1000px;
    }
}

</style>