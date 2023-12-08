<script>
export default {
    name: 'HeaderMenuComponent',
    data() {
        return {
            menu: [
                { name: 'Characters', link: '#' },
                { name: 'Comics', link: '#' },
                { name: 'Movies', link: '#' },
                { name: 'TV', link: '#' },
                { name: 'Games', link: '#' },
                { name: 'Collectibles', link: '#' },
                { name: 'Videos', link: '#' },
                { name: 'Fans', link: '#' },
                { name: 'News', link: '#' },
                { name: 'Shop', link: '#' },
            ]
        }
    }
}
</script>


<template>
    <div class="header-menu">
        <ul>
            <li v-for="item in menu">{{ item.name }}</li>
        </ul>
    </div>
</template>



<style scoped lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: $primary-text-color;

}

li {
    padding: 3.125rem 0.125rem;
    margin-right: 1.8rem;
    cursor: pointer;
    text-transform: uppercase;
    font-weight: bold;
    position: relative;

    &:hover {
        color: $brand-blue;
    }

    //pseudo-element under the link to show at the end of the link
    &:hover::after {
        content: '';
        display: block;
        position: absolute;
        bottom: 0px;
        left: 0;
        width: 100%;
        height: 0.3rem;
        background-color: $brand-blue;
    }
}
</style>
