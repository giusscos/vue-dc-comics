<template>
    <ul class="nav_list uppercase">
        <li class="list_item" v-for="(navLink, i) in navLinks" :key="`${i}nav`" :class="navLink.currentStatus">
            <a class="item_link" :href="navLink.href">
                {{ navLink.text }}
            </a>
        </li>
    </ul>
</template>
<script>
const navLinks = [
    {
        href: '#',
        text: 'Characters',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'Comics',
        currentStatus: 'active',
    },
    {
        href: '#',
        text: 'Movies',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'Tv',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'Games',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'Collectibles',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'Videos',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'Fans',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'News',
        currentStatus: '',
    },
    {
        href: '#',
        text: 'Shop',
        currentStatus: ''
    },
]
export default {
    data() {
        return {
            navLinks
        }
    }
}
</script>
<style lang="scss" scoped>
@import '../style/variables';

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
</style>