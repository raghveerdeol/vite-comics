<script>
import AppSignUp from './AppSignUp.vue';
export default {
data() {
    return {
        dcComixLinks: [
            {
                id: 1,
                title: "characters",
                url: "#",
            },
            {
                id: 2,
                title: "comics",
                url: "#",
            },
            {
                id: 3,
                title: "movies",
                url: "#",
            },
            {
                id: 4,
                title: "tv",
                url: "#",
            },
            {
                id: 5,
                title: "games",
                url: "#",
            },
            {
                id: 6,
                title: "videos",
                url: "#",
            },
            {
                id: 7,
                title: "news",
                url: "#",
            },
        ],
        shopLinks: [
            {
                id: 1,
                title: "Shop DC",
                url: "#"
            },
            {
                id: 2,
                title: "Shop DC Collectibles",
                url: "#"
            },
        ],
        dcLinks: [
            {
                id: 1,
                title: "Terms of Use",
                url: "#",
            },
            {
                id: 2,
                title: "Privacy policy(New)",
                url: "#",
            },
            {
                id: 3,
                title: "Ad Choices",
                url: "#",
            },
            {
                id: 4,
                title: "Advertising",
                url: "#",
            },
            {
                id: 5,
                title: "Jobs",
                url: "#",
            },
            {
                id: 6,
                title: "Subscriptions",
                url: "#",
            },
            {
                id: 7,
                title: "Talent Workshops",
                url: "#",
            },
            {
                id: 8,
                title: "CPSC Certificates",
                url: "#",
            },
            {
                id: 9,
                title: "Ratings",
                url: "#",
            },
            {
                id: 10,
                title: "Shop Help",
                url: "#",
            },
            {
                id: 11,
                title: "Contact Us",
                url: "#",
            },
            
        ],
        sitesLinks: [
            {
                id: 1,
                title: "DC",
                url: "#",
            },
            {
                id: 2,
                title: "MAD Magazine",
                url: "#",
            },
            {
                id: 3,
                title: "DC Kids",
                url: "#",
            },
            {
                id: 4,
                title: "DC Universe",
                url: "#",
            },
            {
                id: 5,
                title: "DC Powe Visa",
                url: "#",
            },
            
        ],
    }
},
components: {
    AppSignUp,
}
}
</script>

<template>
    <section>
        <div class="footer-link">
            <div class="links">
                <div>
                    <h2>
                        dc comics
                    </h2>
                    <ul class="dc-comics">
                        <li v-for="(link, index) in dcComixLinks" :key="link.id">
                            {{ link.title }}
                        </li>
                    </ul>
                </div>
                <div>
                    <h2>
                        shop
                    </h2>
                    <ul class="shop">
                        <li v-for="(link, index) in shopLinks" :key="link.id">
                            {{ link.title }}
                        </li>
                    </ul>
                </div>
                <div>
                    <h2>
                        dc
                    </h2>
                    <ul class="dc">
                        <li v-for="(link, index) in dcLinks" :key="link.id">
                            {{ link.title }}
                        </li>
                    </ul>
                </div>
                <div>
                    <h2>
                        sites
                    </h2>
                    <ul class="sites">
                        <li v-for="(link, index) in sitesLinks" :key="link.id">
                            {{ link.title }}
                        </li>
                    </ul>
                </div>
            </div>
    
            <div class="logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
        <AppSignUp/>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
.footer-link{
    background-color: black;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    color: white;
    height: 375px;
    @include flex-around();
    @include padFooter();
    overflow: hidden;
        div{
            width: 50%;
        };
}
.links{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 100%;
    padding: 3rem 0;
        div{
            width: calc((100% / 3) - 4px);
        };
}
h2{
    padding: 12px 0;
    text-transform: uppercase;
    font-size: 1.2rem;
}
li{
    line-height: 20px;
    font-size: 14px;
    color: grey;
}
</style>