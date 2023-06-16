<template>
    <li>
        {{ elementComics.series }}
    </li>
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
        margin-right: 1.5rem;
        font-size: 0.65rem;
        font-weight: 600;

        &:hover{
            text-decoration: underline;
        }
    }
}

</style>