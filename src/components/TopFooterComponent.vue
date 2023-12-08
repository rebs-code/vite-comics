<script>
export default {
    name: 'TopFooterComponent',
    data() {
        return {
            footerData: [
                {
                    title: 'DC Comics',
                    links: [
                        { name: 'Characters', link: '#' },
                        { name: 'Comics', link: '#' },
                        { name: 'Movies', link: '#' },
                        { name: 'TV', link: '#' },
                        { name: 'Games', link: '#' },
                        { name: 'Collectibles', link: '#' },
                        { name: 'Videos', link: '#' },
                        { name: 'News', link: '#' },

                    ]
                },
                {
                    title: 'Shop',
                    links: [
                        {
                            name: 'Shop DC',
                            url: '#'
                        },
                        {
                            name: 'Shop DC Collectibles',
                            url: '#'
                        },
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        {
                            name: 'Terms Of Use',
                            url: '#'
                        },
                        {
                            name: 'Privacy Policy (New)',
                            url: '#'
                        },
                        {
                            name: 'Ad Choices',
                            url: '#'
                        },
                        {
                            name: 'Advertising',
                            url: '#'
                        },
                        {
                            name: 'Jobs',
                            url: '#'
                        },
                        {
                            name: 'Subscriptions',
                            url: '#'
                        },
                        {
                            name: 'Talent Workshops',
                            url: '#'
                        },
                        {
                            name: 'CPSC Certificates',
                            url: '#'
                        },
                        {
                            name: 'Ratings',
                            url: '#'
                        },
                        {
                            name: 'Shop Help',
                            url: '#'
                        },
                        {
                            name: 'Contact Us',
                            url: '#'
                        },

                    ]
                },
                {
                    title: 'Sites',
                    links: [
                        {
                            name: 'DC',
                            url: '#'
                        },
                        {
                            name: 'MAD Magazine',
                            url: '#'
                        },
                        {
                            name: 'DC Kids',
                            url: '#'
                        },
                        {
                            name: 'DC Universe',
                            url: '#'
                        },
                        {
                            name: 'DC Power Visa',
                            url: '#'
                        },
                    ]
                },
            ]
        }
    },

}
</script>

<template>
    <div class="top-footer">
        <div class="top-footer-container">
            <div class="footer-menu">
                <ul>
                    <li v-for="item in footerData">
                        <h3>{{ item.title }}</h3>
                        <ul>
                            <li v-for="link in item.links">
                                <a :href="link.url">{{ link.name }}</a>
                            </li>
                        </ul>
                    </li>
                </ul>
            </div>
            <div class="footer-logo">
                <img src="../img/dc-logo-bg.png" alt="DC Logo">
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

.top-footer {
    background-image: url('../img/footer-bg.jpg');
    padding: 40px 0;
    color: white;

    a {
        text-decoration: none;
        color: $text-gray;
    }
}

.top-footer-container {
    max-width: 1270px;
    margin: 0 auto;
    border: 1px solid white;
    display: flex;
}

ul {
    list-style: none;
    padding: 0;
    margin: 0;
}

div>ul {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    max-height: 400px;

}

div>ul>li {
    padding-bottom: 30px;
}

div>ul>li>h3 {
    font-size: 18px;
    font-weight: bold;
    padding-bottom: 20px;
    text-transform: uppercase;
}

div>ul>li>ul>li {
    padding-bottom: 10px;
    font-size: 13px;
    padding-right: 30px;
}
</style>