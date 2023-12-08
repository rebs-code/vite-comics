<script>
import TopFooterComponent from './TopFooterComponent.vue';
import BottomFooterComponent from './BottomFooterComponent.vue';

export default {
    name: 'FooterComponent',
    components: {
        TopFooterComponent,
        BottomFooterComponent
    }

}
</script>

<template>
    <footer>
        <TopFooterComponent></TopFooterComponent>
        <BottomFooterComponent></BottomFooterComponent>
    </footer>
</template>

<style scoped lang="scss">
footer {
    padding: 0;
    margin: 0;
}
</style>
