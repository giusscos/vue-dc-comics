<template>
    <header>
        <div class="container">
            <div class="logo_wrapper">
                <img src="../assets/img/dc-logo.png" alt="logo-dc" />
            </div>
            <nav class="main_nav">
                <NavLinks />
            </nav>
        </div>
    </header>
</template>

<script>
import NavLinks from "./NavLinks.vue";
export default{
    components: { NavLinks }
}
</script>

<style lang="scss" scoped>
header {
    .container {
        display: flex;
        padding: 0.5rem 0.75rem 0;

        .logo_wrapper {
            margin-right: auto;
        }
    }
}
</style>
