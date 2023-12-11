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
        <div class="blue-stripe-container container-large">
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
@use '../assets/scss/partials/variables' as *;


.blue-stripe {
    background-color: $brand-blue;
    color: white;
    text-transform: uppercase;
}

.blue-stripe-container {
    width: 100%;
    padding: 3.125rem;
    font-size: 0.75rem;
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
    padding: 0 0.3rem;
    display: flex;
    align-items: center;

    img {
        max-height: 3.4rem;
        width: auto;
        margin-right: 0.93rem;
    }

    img[alt="power-visa"] {
        max-height: 2.5rem;
    }
}
</style>
        