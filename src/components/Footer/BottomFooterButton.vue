<script>
export default {
    name: 'BottomFooterButton',

}
</script>

<template>
    <div class="bottom-footer-left">
        <button>Sign-up Now!</button>
    </div>
</template>

<style scoped lang="scss">
@use '../../assets/scss/partials/variables' as *;

button {
    background-color: transparent;
    color: white;
    padding: .9375rem;
    border: 2px solid $brand-blue;
    font-size: 1.1rem;
    text-transform: uppercase;
    font-weight: 700;
    cursor: pointer;
}
</style>