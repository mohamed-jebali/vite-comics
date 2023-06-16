<template>
    <div class="container-card">
        <img :src="elementComics.thumb" alt="images-comics">
        <p>
            {{ elementComics.series }}
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
    
    margin-bottom: 1rem;
    width: calc(100% / 6 );

    img{
            height: 180px;
            width: 150px;
            object-fit: cover;
        }
}
p{
        
        margin-right: 1.5rem;
        font-size: 0.85rem;

        &:hover{
            text-decoration: underline;
        }
    }


</style>