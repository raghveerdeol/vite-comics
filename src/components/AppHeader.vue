<script>
export default {
data() {
    return {
        navLinks: [
            {
                id: 1,
                title: "characters",
                url: "#",
                active: false,
            },
            {
                id: 2,
                title: "comics",
                url: "#",
                active: true,
            },
            {
                id: 3,
                title: "movies",
                url: "#",
                active: false,
            },
            {
                id: 4,
                title: "tv",
                url: "#",
                active: false,
            },
            {
                id: 5,
                title: "games",
                url: "#",
                active: false,
            },
            {
                id: 6,
                title: "collectibles",
                url: "#",
                active: false,
            },
            {
                id: 7,
                title: "videos",
                url: "#",
                active: false,
            },
            {
                id: 8,
                title: "fans",
                url: "#",
                active: false,
            },
            {
                id: 9,
                title: "news",
                url: "#",
                active: false,
            },
            {
                id: 10,
                title: "shop",
                url: "#",
                active: false,
            },
        ]
    }
}
}
</script>

<template>
    <div>
        <section class="main-logo">
            <img src="../assets/img/dc-logo.png" alt="main logo DC">
        </section>
    
        <nav class="nav-bar">
            <ul>
                <li v-for="link in navLinks" :key="link.id">
                    <a href="link.url">
                        {{ link.title }}
                    </a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
</style>