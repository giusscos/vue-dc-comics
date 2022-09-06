<template>
    <div class="banner menu">
        <div class="container">
            <div class="footer_menu">
                <div class="menu_item" v-for="(footerLink, i) in footerLinks" :key="`${i}footer`">
                    <h3 class="item_title">
                        {{ footerLink.title}}
                    </h3>
                    <ul class="item_list-wrapper">
                        <li class="list_item" v-for="(link, j) in footerLink.links" :key="`${j}link`">
                            <a :href="link.href" class="item_link">
                                {{ link.text}}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
const footerLinks = [
    {
        title: 'Dc comics',
        links: [
            {
                href: '#',
                text: 'Characters'
            },
            {
                href: '#',
                text: 'Comics'
            },
            {
                href: '#',
                text: 'Movies'
            },
            {
                href: '#',
                text: 'Tv'
            },
            {
                href: '#',
                text: 'Games'
            },
            {
                href: '#',
                text: 'Videos'
            },
            {
                href: '#',
                text: 'News'
            },
        ]
    },
    {
        title: 'Dc',
        links: [
            {
                href: '#',
                text: 'Terms of use'
            },
            {
                href: '#',
                text: 'Privacy policy (New)'
            },
            {
                href: '#',
                text: 'Ad Choices'
            },
            {
                href: '#',
                text: 'Advertising'
            },
            {
                href: '#',
                text: 'Jobs'
            },
            {
                href: '#',
                text: 'Subscriptions'
            },
            {
                href: '#',
                text: 'Talent Workshops'
            },
            {
                href: '#',
                text: 'CPSC Certificates'
            },
            {
                href: '#',
                text: 'Ratings'
            },
            {
                href: '#',
                text: 'Shop help'
            },
            {
                href: '#',
                text: 'Contact us'
            },
        ]
    },
    {
        title: 'Sites',
        links: [
            {
                href: '#',
                text: 'Dc'
            },
            {
                href: '#',
                text: 'MAD Magazine'
            },
            {
                href: '#',
                text: 'DC Kids'
            },
            {
                href: '#',
                text: 'DC Universe'
            },
            {
                href: '#',
                text: 'DC Power visa'
            },
        ]
    },
    {
        title: 'Shop',
        links: [
            {
                href: '#',
                text: 'Shop DC'
            },
            {
                href: '#',
                text: 'Shop DC Collectibles'
            }
        ]
    },
]
export default {
    data() {
        return {
            footerLinks
        }
    }
}
</script>
<style lang="scss" scoped>
@import '@/style/variables';

.banner {
    &.menu {
        color: $dc-light_bg;
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        background-image: url(../../assets/img/footer-bg.jpg);

        .container {
            display: flex;

            background-size: auto 130%;
            background-repeat: no-repeat;
            background-position: center right;
            background-image: url(../../assets/img/dc-logo-bg.png);

            .footer_menu {
                padding: 2rem 0;
                display: flex;
                flex-wrap: wrap;
                column-gap: 1rem;
                margin-right: auto;

                .menu_item {
                    flex-basis: calc((100% / 3) - 1rem);

                    h3 {
                        font-weight: bold;
                        padding-bottom: 1rem;
                        text-transform: uppercase;
                    }

                    .list_item {
                        padding: 0.1rem 0;
                        
                        .item_link {
                            opacity: 0.7;
                            padding: 0.1rem 0;
                            
                            &:hover {
                                opacity: 1;
                            }
                        }
                    }
                }
            }
        }
    }
}
</style>