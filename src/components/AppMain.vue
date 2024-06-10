<script>
import AppShop from './AppShop.vue';

export default {
data() {
    
},
components: {
        AppShop,
    },
}
</script>

<template>
    <div>
        <h1>-->content goes here<--</h1>
    </div>
    
    <AppShop/>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
div{
    background-color: $bg-main;
    color: white;
    @include padMain();
}
</style>