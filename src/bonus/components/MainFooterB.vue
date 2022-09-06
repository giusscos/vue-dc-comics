<template>
    <footer>
        <BannerBlue />
        <FooterMenu />
        <div class="banner join">
            <div class="container">
                <div class="cta_wrapper">
                    <a href="" class="btn sign-up_cta uppercase">
                        Sign up now!
                    </a>
                </div>
                <h3 class="uppercase">
                    Follow us
                </h3>
                <SocialLinks />
            </div>
        </div>
    </footer>
</template>

<script>
import BannerBlue from './BannerBlue.vue';
import FooterMenu from './FooterMenu.vue';
import SocialLinks from './SocialLinks.vue';

export default {
    components: {
        BannerBlue,
        FooterMenu,
        SocialLinks
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/index.scss';
@import '@/style/variables';

footer {
    position: relative;

    .banner {
        &.join {
            padding: 3rem 0;
            color: $dc-light_bg;
            background-color: $dc-dark_bg_alternative;

            .container {
                display: flex;
                align-items: center;

                .btn {
                    &.sign-up_cta {
                        border: 2px solid $dc-accent_link;
                    }
                }

                h3 {
                    font-weight: bold;
                    margin-left: auto;
                    margin-right: 1rem;
                    color: $dc-accent_link;
                }
            }
        }
    }
}
</style>