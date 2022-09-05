<template>
    <header>
        <div class="container">
            <div class="logo_wrapper">
                <img src="@/assets/img/dc-logo.png" alt="logo-dc" />
            </div>
            <nav class="main_nav">
                <ul class="nav_list uppercase">
                    <li class="list_item">
                        <a class="item_link" href="">
                            Characters
                        </a>
                    </li>
                    <li class="list_item active">
                        <a class="item_link" href="">
                            Comics
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            Movies
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            Tv
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            Games
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            Collectibles
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            Videos
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            Fans
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            News
                        </a>
                    </li>
                    <li class="list_item">
                        <a class="item_link" href="">
                            Shop
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

header {
    .container {
        display: flex;
        padding: 0.5rem 0.75rem 0;

        .logo_wrapper {
            margin-right: auto;
        }

        .main_nav {

            .nav_list {
                gap: 1.5rem;
                height: 100%;
                display: flex;

                .list_item {
                    height: 100%;
                    display: flex;
                    position: relative;
                    align-items: center;

                    &.active {
                        .item_link {
                            color: $dc-accent_link;

                            &::after {
                                content: "";
                                position: absolute;
                                bottom: 0;
                                left: 50%;
                                width: 100%;
                                height: 0.5rem;
                                transform: translateX(-50%);
                                background-color: $dc-accent_link;
                            }
                        }
                    }

                    .item_link {
                        font-weight: bold;
                        padding: 1rem 0;

                        &:hover {
                            color: $dc-accent_link;
                        }
                    }
                }
            }
        }
    }
}
</style>
