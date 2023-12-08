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
                            icon: 'fab fa-instagram',
                            url: '#'
                        },
                        {
                            icon: 'fab fa-facebook',
                            url: '#'
                        },
                        {
                            icon: 'fab fa-youtube',
                            url: '#'
                        },
                        {
                            icon: 'fab fa-twitter',
                            url: '#'
                        },
                        {
                            icon: 'fab fa-linkedin',
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
                <li v-for="link in item.links" :key="link.icon">
                    <a :href="link.url">
                        <i :class="link.icon"></i>
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