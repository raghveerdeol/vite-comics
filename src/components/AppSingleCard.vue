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
    <article>
        <img :src="singleComic.thumb" :alt="singleComic.type">
        <h2>
            {{ singleComic.series }}
        </h2>
    </article>
</template>

<style scoped>

</style>