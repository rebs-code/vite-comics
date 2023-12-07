<script>
export default {
    name: 'BlueStripeComponent',
    data() {
        return {
            items: [
                { icon: "buy-comics-digital-comics.png", name: 'digital comics', link: '#' },
                { icon: "buy-comics-merchandise.png", name: 'merchandise', link: '#' },
                { icon: "buy-comics-subscriptions.png", name: 'subscriptions', link: '#' },
                { icon: "buy-comics-shop-locator.png", name: 'shop locator', link: '#' },
                { icon: "buy-dc-power-visa.png", name: 'power-visa', link: '#' },
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
    padding: 50px 0;
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
    padding: 0 10px;

    img {
        width: 50%;
    }

    img[alt="power-visa"] {
        width: 85%;
    }
}
</style>
        