<template lang="">
    <div class='content-container'>
        <div class='title-content mg-auto'>
            <h1>
            -> Content goes here --
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
    background-color: black;
    padding: 4rem;

    h1{
        font-size: 2rem;
    }
    .title-content{
        max-width: 1200px;
    }
}

</style>