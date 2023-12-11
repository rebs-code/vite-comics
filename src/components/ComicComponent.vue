<script>
export default {
    name: 'ComicComponent',
    props: {
        thumb: String,
        series: String,
    },
}

</script>

<template>
    <div>
        <img :src="thumb" :alt="series">
        <h3>{{ series }}</h3>
    </div>
</template>

<style scoped lang="scss"></style>