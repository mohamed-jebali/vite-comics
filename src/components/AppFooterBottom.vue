<template lang="">
    <footer class='content-container'>
        <div class="footer-wrapper-bottom mg-auto">
            <div class='title-content'>
                <button>
                    SIGN-UP NOW !
                </button>
            </div>
            <div class='social-container'>
                <h2>
                    Follow us
                </h2>
                <div class="socials">
                    <img src="../assets/img/footer-facebook.png" alt="facebook-logo">
                    <img src="../assets/img/footer-twitter.png" alt="twitter-logo">
                    <img src="../assets/img/footer-youtube.png" alt="youtube-logo">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest-logo">
                    <img src="../assets/img/footer-periscope.png" alt="periscope-logo">
                </div>
            </div>
        </div>
    </footer>
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


.content-container{
    background-color: $DcFooterBg;
}

.footer-wrapper-bottom{
    padding: 2rem 0rem;
    max-width: 1000px;
    color: white;
    @include flex(row,space-between,center);
    

    button{
        padding: 0.9rem;
        background-color: $DcFooterBg;
        color: white;
        border: 2px solid $DcColorBlue;
    }

    .social-container{
        @include flex(row,space-between,center);
    
        h2{
            color: $DcColorBlue;
            margin-right: 2rem;
        }
        .socials{
            @include flex(row,space-between,center);

            img{
                margin-right: 1rem;
            }
        }
    }
}

</style>