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
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;

.top-footer {
    background-image: url('../img/footer-bg.jpg');
    color: white;
    height: 23.4375rem;
    padding-top: 2.5rem;
}

.top-footer-container {
    max-width: 80rem;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
}
</style>