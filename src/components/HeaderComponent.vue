<script>
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
.header {
    border: 1px solid black;
}

.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 1270px;
    margin: 0 auto;
}
</style>