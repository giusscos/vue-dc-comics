<template>
    <ul class="social_list">
        <li class="list_item" v-for="(socialLink, i) in socialLinks" :key="`${i}social`">
            <a :href="socialLink.href" class="item_link">
                <img :src="socialLink.src" :alt="socialLink.text" />
            </a>
        </li>
    </ul>
</template>
<script>
const socialLinks = [
    {
        href: '#',
        src: require('../assets/img/footer-facebook.png'),
        text: 'Facebook',
    },
    {
        href: '#',
        src: require('../assets/img/footer-twitter.png'),
        text: 'Twitter',
    },
    {
        href: '#',
        src: require('../assets/img/footer-youtube.png'),
        text: 'Youtube',
    },
    {
        href: '#',
        src: require('../assets/img/footer-pinterest.png'),
        text: 'Pinterest',
    },
    {
        href: '#',
        src: require('../assets/img/footer-periscope.png'),
        text: 'Periscope',
    },
]
export default {
    data() {
        return {
            socialLinks
        }
    }
}
</script>
<style lang="scss" scoped>
.social_list {
    display: flex;
    gap: 1rem;
    
    .list_item {

        .item_link {
            opacity: 0.8;
            
            &:hover {
                opacity: 1;
            }
        }
    }
}
</style>