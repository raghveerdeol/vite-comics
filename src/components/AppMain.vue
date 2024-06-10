<script>
export default {
data() {

}
}
</script>

<template>
    <main>
        <h1>-->content goes here<--</h1>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
main{
    background-color: $bg-main;
    color: white;
    @include padMain();
}
</style>