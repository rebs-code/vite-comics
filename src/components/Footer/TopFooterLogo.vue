<script>

export default {
    name: 'TopFooterLogo',
}
</script>

<template>
    <div class="top-footer-logo">
        <img src="../../../img/dc-logo-bg.png" alt="DC Logo">
    </div>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;

.top-footer-logo {
    position: absolute;
    top: -45%;
    left: 50%;
}
</style>
