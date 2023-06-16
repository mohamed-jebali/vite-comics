<template>
    <div class="container-card">
        <img :src="elementComics.thumb" alt="images-comics">
        <p>
            {{ elementComics.series.toUpperCase() }}
        </p>
    </div>
</template>
<script>
import { createApp } from 'vue'
export default{
    name:'AppComics',
    props:{
        elementComics:String
    },

    }

</script>
<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;


div.container-card{
    
    margin-bottom: 4rem;
    width: calc(100% / 6 );

    img{
            height: 160px;
            width: 150px;
        }
}
p{    
        margin-top: 0.8rem;
        margin-right: 1.5rem;
        font-size: 0.7rem;
        width: 160px;

        &:hover{
            text-decoration: underline;
        }
    }


</style>