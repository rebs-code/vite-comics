<script>
export default {
    name: 'BottomFooterMenu',
    data() {
        return {
            menuItems: [
                {
                    title: 'Follow Us',
                    links: [
                        {
                            icon: 'footer-facebook.png',
                            url: '#'
                        },
                        {
                            icon: 'footer-twitter.png',
                            url: '#'
                        },
                        {
                            icon: 'footer-youtube.png',
                            url: '#'
                        },
                        {
                            icon: 'footer-pinterest.png',
                            url: '#'
                        },
                        {
                            icon: 'footer-periscope.png',
                            url: '#'
                        }
                    ]
                }
            ]
        }
    }
}
</script>

<template>
    <div class="bottom-footer-menu">
        <div class="bottom-footer-menu-item" v-for="item in menuItems">
            <h3>{{ item.title }}</h3>
            <ul>
                <li v-for="link in item.links">
                    <a :href="link.url">
                        <img :src="`/img/${link.icon}`" :alt="link.icon">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;

.bottom-footer-menu-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

h3 {
    font-size: 1.1rem;
    font-weight: 700;
    text-transform: uppercase;
    color: $brand-blue;
}


ul {
    list-style: none;
    display: flex;
}

li {
    padding-left: 1.25rem;
    display: flex;
    align-items: center;
}
</style>