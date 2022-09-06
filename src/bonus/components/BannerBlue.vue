<template>
    <div class="banner blue">
        <div class="container">
            <ul class="footer_list-merch uppercase">
                <li class="list_item" v-for="(bannerLink, i) in bannerLinks" :key="`${i}banner`">
                    <a :href="bannerLink.href" class="item_link">
                        <img :src="bannerLink.src" :alt="bannerLink.text" :height="bannerLink.height" />
                        {{ bannerLink.text }}
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
    const bannerLinks = [
        {
            src: require('../../assets/img/buy-comics-digital-comics.png'),
            text: 'Digital comics',
            href: '#',
            height: '70px',
        },
        {
            src: require('../../assets/img/buy-comics-merchandise.png'),
            text: 'Dc merchandise',
            href: '#',
            height: '70px',
        },
        {
            src: require('../../assets/img/buy-comics-subscriptions.png'),
            text: 'Subscription',
            href: '#',
            height: '70px',
        },
        {
            src: require('../../assets/img/buy-comics-shop-locator.png'),
            text: 'Comic shop location',
            href: '#',
            height: '70px',
        },
        {
            src: require('../../assets/img/buy-dc-power-visa.svg'),
            text: 'Dc power visa',
            href: '#',
            height: '50px',
        },
    ]
export default {
    data(){
        return {
            bannerLinks
        }
    }
}
</script>
<style lang="scss" scoped>
@import '../../style/index.scss';
@import '../../style/variables';

.banner {
    &.blue {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        background-color: $dc-accent_link;

        .container {
            .footer_list-merch {
                padding: 3rem 2rem;
                display: flex;
                align-items: center;

                .list_item {
                    flex-grow: 1;

                    .item_link {
                        gap: 1rem;
                        display: flex;
                        font-size: 0.85rem;
                        font-weight: bold;
                        align-items: center;
                        color: $dc-light_bg;
                    }
                }
            }
        }
    }
}
</style>