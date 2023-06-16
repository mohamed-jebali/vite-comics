<template>
    <div class="container">
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


.container{
    width: 70%;
    display: flex;
    flex-wrap: wrap;
}



div{
    width: calc(100% / 6);
    img{
            height: 200px;
        }
}
p{
        
        margin-right: 1.5rem;
        font-size: 0.65rem;
        font-weight: 600;

        &:hover{
            text-decoration: underline;
        }
    }

</style>