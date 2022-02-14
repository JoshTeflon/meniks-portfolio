<script>
    import LogoSvg from "./icons/LogoSvg.vue";

    export default {
        name: "Nav",
        components: { LogoSvg }
    }
</script>

<template>
    <div class="nav">
        <div class="nav--content">
            <div class="mk--logo">
                <LogoSvg />
            </div>
            <ul class="nav-items">
                <li>Home</li>
                <li>Projects</li>
                <li>Contact</li>
            </ul>
            <button class="nav-icon">
                <div class="icon-bar"></div>
                <div class="icon-bar"></div>
                <div class="icon-bar"></div>
            </button>
        </div>
    </div>
</template>

<style scoped>
    .nav {
        width: 80%;
        margin: 0 auto;
        padding: 2rem 0;
        height: 15vh;
        /* position: absolute;
        top: 0; */
    }

    .nav .nav--content {
        position: relative;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .nav .mk--logo {
        width: 3rem;
    }

    .nav .nav-items {
        display: none;
        align-items: center;
        list-style: none;
        font-size: 1rem;
        color: #a9a9a9;
    }

    .nav .nav-items li {
        margin-left: 3rem;
    }

    .nav .nav--content .nav-icon {
        display: flex;
        justify-content: space-between;
        width: 2rem;
        border: none;
        background: var(--mk-c-blue-1);
        cursor: pointer;
    }

    .nav .nav--content .nav-icon .icon-bar {
        height: 2rem;
        transition: 0.3s ease-in-out;
    }

    .nav .nav--content .nav-icon .icon-bar:nth-child(2) {
        height: 1.5rem;
    } 

            /*
            }

            .nav_open {

                .bar {

                    &:nth-child(1) {
                        transform: translateX(8px) rotate(-45deg);

                        @include responsive(tablet-md) {
                            transform: translateX(9px) rotate(-45deg);
                        }

                        @include responsive(tablet-lg) {
                            transform: translateX(12px) rotate(-45deg);
                        }

                        @include responsive(desktop) {
                            transform: translateX(15px) rotate(-45deg);
                        }
                    }

                    &:nth-child(2) {
                        display: none;
                    }

                    &:nth-child(3) {
                        transform: translateX(-8px) rotate(45deg);

                        @include responsive(tablet-md) {
                            transform: translateX(-9px) rotate(45deg);
                        }

                        @include responsive(tablet-lg) {
                            transform: translateX(-12px) rotate(45deg);
                        }

                        @include responsive(desktop) {
                            transform: translateX(-15px) rotate(45deg);
                        }
                    }
                } */


    @media screen and (min-width: 640px) {
        .nav .nav-items {
            display: flex;
        }

        .nav .nav--content .nav-icon {
            display: none;
        }
    }
</style>