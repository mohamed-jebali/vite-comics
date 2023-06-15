<template>
    <div class='content-container'>
        <ul class='list-content mg-auto'>
            <li>
                <img src='../assets/img/buy-comics-digital-comics.png' alt='list-image-bonus'>
                <a href="#">
                    DIGITAL COMICS
                </a>
            </li>
            <li>
                <img src='../assets/img/buy-comics-merchandise.png' alt='list-image-bonus'>
                <a href="#">
                    DC MERCHANDISE
                </a>
            </li>
            <li>
                <img src='../assets/img/buy-comics-subscriptions.png' alt='list-image-bonus'>
                <a href="#">
                    SUBSCRIPTION
                </a>
            </li>
            <li>
                <img src='../assets/img/buy-comics-shop-locator.png' alt='list-image-bonus'>
                <a href="#">
                    COMIC SHOP LOCATOR
                </a>
            </li>
            <li>
                <img class="power-visa" src='../assets/img/buy-dc-power-visa.svg' alt='list-image-bonus'>
                <a href="#">
                    DC POWER VISA
                </a>
            </li>
        </ul>
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
    padding: 1rem 0;
    .list-content{
        max-width: 1000px;
        display: flex;
        justify-content: space-between;

        li{
            display: flex;
            align-items: center;

            img{
                margin-right: 1rem;
                height: 40%;
            }
            .power-visa{
                height: 25%;
            }
            a{
                font-size: 0.8rem;
                color: white;
            }
        }
    }
}

</style>