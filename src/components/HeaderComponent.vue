<template>
    <nav class="header center">
        <div class="container header__flex">
            <div class="header__left">                
                    <a class="header__left__logo" href="/index.html"><img src="../assets/img/Logo.svg" alt="переход на главную старницу"></a>
                    <p class="header__left__title">Interno</p>
            </div>
            <div class="header__right">
                <a href="">Home</a>
                <a href="">Project</a>
                <a href="/blog/blogIndex.html">Blog</a>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
@mixin flexSBcenter($gap) {
    display: flex;
    justify-content: space-between;
    gap: $gap;
    align-items: center;
}
.header{
    
    margin-top: 44px;
   
    &__flex{
        @include flexSBcenter(none);
    }


    &__left{
        display: flex;
        justify-content: flex-start;
        gap:8px;
        align-items: center;
        &__logo{

        }
        &__title{
            color: rgb(41, 47, 54);
            font-family: DM Serif Display;
            font-size: 40px;
            font-weight: 400;
            line-height: 125%;
            letter-spacing: 0em;
            text-align: left;
        }
    }
    &__right{
        display: flex;
        justify-content: flex-end;
        gap:40px;
        align-items: center;
        
        color: rgb(41, 47, 54);
        font-family: Jost;
        font-size: 20px;
        font-weight: 400;
        line-height: 125%;
        letter-spacing: 0em;
        text-align: center;

    }

}
</style>
