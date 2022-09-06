<template>
    <main>
        <JumboTron />
        <div class="series_wrapper container">
            <div class="btn info_btn uppercase">
                Current series
            </div>
            <CardSeries />
            <div class="btn viewer_btn uppercase">
                Load more
            </div>
        </div>
    </main>
</template>

<script>
import JumboTron from './JumboTron.vue';
import CardSeries from './CardSeries.vue';

export default {
    components: {
        JumboTron,
        CardSeries
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

main {
    font-weight: bold;
    color: $dc-light_bg;
    background-color: $dc-dark_bg;

    .series_wrapper {
        padding: 1rem;
        display: flex;
        flex-direction: column;
        position: relative;

        .btn {
            &.info_btn {
                font-size: 1.25rem;
                font-weight: bold;
                position: absolute;
                top: 0;
                transform: translateY(-50%);
                background-color: $dc-accent_link;
            }

            &.viewer_btn {
                opacity: 1;
                cursor: pointer;
                align-self: center;
                font-size: 0.85rem;
                font-weight: bold;
                padding: 0.5rem 2rem;
                background-color: $dc-accent_link;
            }
        }
    }
}
</style>