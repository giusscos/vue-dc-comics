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
                <ul class="social_list">
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="../../assets/img/footer-facebook.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="../../assets/img/footer-twitter.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="../../assets/img/footer-youtube.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="../../assets/img/footer-pinterest.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="../../assets/img/footer-periscope.png" alt="" />
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
import BannerBlue from './BannerBlue.vue';
import FooterMenu from './FooterMenu.vue';
export default {
    components: { BannerBlue, FooterMenu}
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

                .social_list {
                    display: flex;
                    gap: 1rem;
                }
            }
        }
    }
}
</style>