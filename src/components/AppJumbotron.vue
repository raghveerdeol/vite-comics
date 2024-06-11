<script>
export default {
data() {
return {

}
}
}
</script>

<template>
    <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="teen titans">
        <span>current series</span>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
    .jumbotron{
        max-width: 100%;
            img{    
                width: 100%;
                max-height: 320px;
                object-fit: cover;
                object-position: top;
            }
            span{
                position: relative;
                bottom: 15px;
                left: 140px;
                background-color: $bg-logo;
                padding: .7rem 2rem;
                text-transform: uppercase;
                font-weight: 900;
                }
    }
</style>