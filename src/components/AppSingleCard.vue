<script>
export default {
data() {
return {

}
},
props: {
    singleComic: {
        type: Object,
        required: true,
    }
}
}
</script>

<template>
    <article class="card">
        <img :src="singleComic.thumb" :alt="singleComic.type">
        <h5>
            {{ singleComic.series }}
        </h5>
    </article>
</template>

<style  lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
.card{
    width: calc((100% / 6) - 1.2rem);
    padding-bottom: 2.5rem;
        img{
            width: 100%;
            height: 200px;
            object-fit: cover;
            object-position: top;
            padding-bottom: 1rem;
        }
        h5{
            text-transform: uppercase;
            font-weight: 100;
        }
}

</style>