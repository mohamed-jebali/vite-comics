<template>
    <div class='jumbo'>

    </div>
</template>


<script>
import { createApp } from 'vue'
export default{

}

</script>


<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;

.jumbo{
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    width: 100%;
    height: 350px;
}

</style>