<script>
import BottomFooterLeft from './BottomFooterLeft.vue';
export default {
    name: 'BottomFooterComponent',
    components: {
        BottomFooterLeft
    }
}
</script>

<template>
    <div class="bottom-footer">
        <div class="bottom-footer-container">
            <BottomFooterLeft />
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;

.bottom-footer {
    background-color: $footer-bg;
    padding: 2rem 0;
}

.bottom-footer-container {
    max-width: 80rem;
    margin: 0 auto;
}
</style>