<script>
import TopFooterMenuComponent from './TopFooterMenuComponent.vue';
import TopFooterLogo from './TopFooterLogo.vue';
export default {
    name: 'TopFooterComponent',

    components: {
        TopFooterMenuComponent,
        TopFooterLogo
    }
}
</script>

<template>
    <div class="top-footer">
        <div class="top-footer-container">
            <TopFooterMenuComponent />
            <TopFooterLogo />
        </div>
    </div>
</template>

<style scoped lang="scss">
.top-footer {
    background-image: url('../img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    color: white;
    height: 23.4375rem;
    padding-top: 2.5rem;
    overflow: hidden;
}

.top-footer-container {
    max-width: 80rem;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    position: relative;
}
</style>