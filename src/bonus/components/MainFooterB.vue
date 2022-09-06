<template>
    <footer>
        <BannerBlue />
        <div class="banner menu">
            <div class="container">
                <menu class="main_menu">
                    <li class="menu_item">
                        <h3 class="item_title">
                            Dc comics
                        </h3>
                        <ul class="item_list-wrapper">
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </li>
                    <li class="menu_item">
                        <h3 class="item_title">
                            Dc
                        </h3>
                        <ul class="item_list-wrapper">
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </li>
                    <li class="menu_item">
                        <h3 class="item_title">
                            Sites
                        </h3>
                        <ul class="item_list-wrapper">
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </li>
                    <li class="menu_item">
                        <h3 class="item_title">
                            Shop
                        </h3>
                        <ul class="item_list-wrapper">
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                            <li class="list_item">
                                <a href="" class="item_link">
                                    Link
                                </a>
                            </li>
                        </ul>
                    </li>
                </menu>
                <div class="logo_wrapper">
                    <img src="@/assets/img/dc-logo-bg.png" alt="" />
                </div>
            </div>
        </div>
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
                            <img src="@/assets/img/footer-facebook.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="@/assets/img/footer-twitter.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="@/assets/img/footer-youtube.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="@/assets/img/footer-pinterest.png" alt="" />
                        </a>
                    </li>
                    <li class="list_item">
                        <a href="" class="item_link">
                            <img src="@/assets/img/footer-periscope.png" alt="" />
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
import BannerBlue from './BannerBlue.vue';
export default {
    components: { BannerBlue }
}
</script>

<style lang="scss" scoped>
@import '@/style/index.scss';
@import '@/style/variables';

footer {
    position: relative;

    .banner {
        &.menu {
            color: $dc-light_bg;
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-image: url(@/assets/img/footer-bg.jpg);

            .container {
                padding: 5rem 0;
                display: flex;
                align-items: center;

                .main_menu {
                    display: flex;
                    flex-wrap: wrap;
                    column-gap: 1rem;
                    margin-right: auto;
                    flex-basis: calc(100% / 3);

                    .menu_item {
                        flex-basis: calc((100% / 3) - 1rem);

                        h3 {
                            font-weight: bold;
                            padding-bottom: 1rem;
                            text-transform: uppercase;
                        }
                    }

                }
            }
        }
    }

    .banner {
        &.join {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
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