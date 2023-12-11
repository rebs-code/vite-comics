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
        <div class="top-footer-container container-large">
            <TopFooterMenuComponent />
            <TopFooterLogo />
        </div>
    </div>
</template>

<style scoped lang="scss">
@import '../../assets/scss/partials/mixins';

.top-footer {
    @include bgImage('../img/footer-bg.jpg', 'center', 'no-repeat');
    color: white;
    height: 23.4375rem;
    padding-top: 2.5rem;
    overflow: hidden;


}

.top-footer-container {
    display: flex;
    justify-content: space-between;
    position: relative;
}
</style>