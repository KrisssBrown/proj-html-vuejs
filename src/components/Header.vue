<template>
    <div class="container nav-bar">
        <a href="#" class="logo">
            <img src="/logo.png">
        </a>

        <ul class="nav-menu">
            <li class="nav-item" v-for="navItem in navMenu" :key="i">
                <a href="#">{{ navItem }}</a>
            </li>
            <li>|</li>
            <i class="fa fa-search" aria-hidden="true"></i>
        </ul>
    </div>
</template>

<!-- ************************************************************************** -->

<script>
export default {
    data() {
        return {
            navMenu: [
                'HOME',
                'PAGES',
                'PROGRAM',
                'TICKETS',
                'SPEAKERS',
                'PAPERS',
                'BLOG',
                'SHORTCODES',

            ]
        }
    },
}
</script>

<!-- ************************************************************************** -->

<style lang="scss" scoped>
.nav-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 110px;

    .nav-menu {
        display: flex;
        gap: 20px;
        align-items: center;
        padding: 10px;
        font-size: 11px;
        font-weight: 700;
        line-height: 40px;
        opacity: 0.5;



        .nav-item:hover {
            color: red;
            border-bottom: 2px solid red;
        }
    }
}
</style>