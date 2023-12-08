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
</style>