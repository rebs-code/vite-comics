<script>
export default {
    name: 'BlueStripeComponent',
    data() {
        return {
            items: [
                { icon: "buy-comics-digital-comics.png", name: 'digital comics', link: '#', text: 'Digital Comics' },
                { icon: "buy-comics-merchandise.png", name: 'merchandise', link: '#', text: 'Merchandise' },
                { icon: "buy-comics-subscriptions.png", name: 'subscriptions', link: '#', text: 'Subscriptions' },
                { icon: "buy-comics-shop-locator.png", name: 'shop locator', link: '#', text: 'Comic Shop Locator' },
                { icon: "buy-dc-power-visa.png", name: 'power-visa', link: '#', text: 'DC Power Visa' },
            ]

        }
    },
}
</script>

<template>
    <div class="blue-stripe">
        <div class="blue-stripe-container">
            <ul>
                <li v-for="item in items">
                    <img :src="`/img/${item.icon}`" :alt="item.name">
                    <p>{{ item.text }}</p>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

.blue-stripe {
    background-color: $brand-blue;
    color: white;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 1px;
    border-bottom: 1px solid $brand-blue;
}

.blue-stripe-container {
    width: 100%;
    max-width: 1270px;
    margin: 0 auto;
    padding: 50px 50px;
    font-size: 12px;
}

ul {
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0;
    margin: 0;
}

li {
    padding: 0 5px;
    display: flex;
    align-items: center;

    img {
        max-height: 55px;
        width: auto;
        margin-right: 15px;
    }

    img[alt="power-visa"] {
        max-height: 40px;
    }
}
</style>
        