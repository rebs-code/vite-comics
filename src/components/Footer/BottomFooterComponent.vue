<script>
import BottomFooterButton from './BottomFooterButton.vue';
import BottomFooterMenu from './BottomFooterMenu.vue';
export default {
    name: 'BottomFooterComponent',
    components: {
        BottomFooterButton,
        BottomFooterMenu
    }
}
</script>

<template>
    <div class="bottom-footer">
        <div class="bottom-footer-container">
            <BottomFooterButton />
            <BottomFooterMenu />
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../../assets/scss/partials/variables' as *;

.bottom-footer {
    background-color: $footer-bg;
    padding: 1.875rem 0;
}

.bottom-footer-container {
    max-width: 1280px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>