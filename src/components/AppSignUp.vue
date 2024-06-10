<script>
export default {
data() {
    return{
        icons: [
            {
                id: 1,
                img: '../src/assets/img/footer-facebook.png',
                active: false,
            },
            {
                id: 2,
                img: '../src/assets/img/footer-twitter.png',
                active: false,
            },
            {
                id: 3,
                img: '../src/assets/img/footer-youtube.png',
                active: false,
            },
            {
                id: 4,
                img: '../src/assets/img/footer-pinterest.png',
                active: false,
            },
            {
                id: 5,
                img: '../src/assets/img/footer-periscope.png',
                active: false,
            },
            
        ]
    }
}
}
</script>

<template>
    <div class="socials">
        <div>
            <button>sign-up now!</button>
        </div>
        <div class="social-icons">
            <h2>follow us</h2>
            <ul>
                <li v-for="icon in icons" :key="icon.id">
                    <img :src="icon.img" alt="">
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
.socials{
    @include flex-between();
    padding: 2rem 10rem;
    background-color: $bg-footer;
}
.social-icons{
    @include flex-between();
    ul{
    @include flex-between();
    }
}
h2{
    color: $bg-logo;
    margin-right: 2rem;
    font-weight: 900;
    text-transform: uppercase;
}
button{
    background-color: $bg-footer;
    border: 2px solid $bg-logo;
    color: white;
    padding: 1rem;
    text-transform: uppercase;
    font-weight: 900;
}
li{
    margin-right: 1.5rem;
}
</style>