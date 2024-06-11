<script>
import AppShop from './AppShop.vue';
import AppJumbotron from './AppJumbotron.vue';
import AppListCards from './AppListCards.vue';

export default {
data() {
    
},
components: {
        AppShop,
        AppJumbotron,
        AppListCards,
    },
}
</script>

<template>
    <AppJumbotron/>
    <div>
        <AppListCards/>
    </div>
    
    <AppShop/>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
div{
    background-color: $bg-main;
    color: white;
}
</style>