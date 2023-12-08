<script>
// @ts-ignore
import LogoComponent from './LogoComponent.vue';
import HeaderMenuComponent from './HeaderMenuComponent.vue';

export default {
    name: 'HeaderComponent',
    components: {
        LogoComponent,
        HeaderMenuComponent
    }
}
</script>



<template>
    <header class="header">
        <div class="header-container">
            <LogoComponent></LogoComponent>
            <HeaderMenuComponent></HeaderMenuComponent>
        </div>
    </header>
</template>

<style scoped>
.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 80rem;
    margin: 0 auto;
}
</style>