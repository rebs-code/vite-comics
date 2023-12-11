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
        </div>
    </div>
</template>

<style scoped lang="scss">
@import '../../assets/scss/partials/mixins';

.top-footer {
    @include bgImage('../../../public/img/footer-bg.jpg', 'center', 'no-repeat');
    background-size: cover;
    color: white;
    height: 375px;
    overflow: hidden;
}

.top-footer-container {
    color: white;
    height: 375px;
    overflow: hidden;
    background-image: url('../../../public/img/dc-logo-bg.png');
    background-position: right;
    background-repeat: no-repeat;
}

.top-footer-container {
    display: flex;
    justify-content: space-between;
    position: relative;
}
</style>