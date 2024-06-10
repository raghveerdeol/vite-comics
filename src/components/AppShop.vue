<script>
export default {
data() {
    return {
        shops: [
            {
                id: 1,
                title: "digital comics",
                img: '../src/assets/img/buy-comics-digital-comics.png',
            },
            {
                id: 2,
                title: "dc merchandise",
                img: '../src/assets/img/buy-comics-merchandise.png',
            },
            {
                id: 3,
                title: "subscription",
                img: '../src/assets/img/buy-comics-subscriptions.png',
            },
            {
                id: 4,
                title: "comic shop locator",
                img: '../src/assets/img/buy-comics-shop-locator.png',
            },
            {
                id: 5,
                title: "dc power visa",
                img: '../src/assets/img/buy-dc-power-visa.svg',
            },
            
        ],
    }
}
}
</script>

<template>
    <div class="cards">
        <ul>
            <li v-for="shop in shops" :key="shop.id">
                <img :src="shop.img" alt="">
                <p>{{ shop.title }}</p>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
    div.cards{
        background-color: $bg-logo;
        color: white;
        text-transform: uppercase;
        @include padMain();
    }
    ul{
        @include flex-around();
    }
    li{
        @include flex-around();
        width: calc((100% / 5) - 2px);
        img{
            width: 50px;
        }
    }
</style>