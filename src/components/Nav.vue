<script>
    import IconEmiSvg from "./icons/IconEmiSvg.vue";

    export default {
        name: "Nav",
        components: { IconEmiSvg }
    }
</script>

<template>
    <div class="nav">
        <div class="nav--content">
            <div class="mk--logo">
                <img src="../assets/EMI logo.svg" />
            </div>
            <ul class="nav-items">
                <li>Home</li>
                <li>Experience</li>
                <li>Testimonials</li>
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
        width: 100%;
        /* margin: 0 auto; */
        padding: 2rem 0;
        /* height: 15vh; */
        position: absolute;
        top: 0;
    }

    .nav .nav--content {
        width: var(--width-mobile);
        margin: 0 auto;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .nav .mk--logo {
        width: 7rem;
    }

    .nav .mk--logo img {
        width: 100%;
    }

    .nav .nav-items {
        display: none;
        align-items: center;
        list-style: none;
        font-size: 0.95rem;
        text-transform: uppercase;
        color: #a9a9a9;
    }

    .nav .nav-items li {
        margin-left: 3rem;
    }

    .nav .nav--content .nav-icon {
        display: flex;
        justify-content: space-between;
        width: 3rem;
        background: transparent;
        border: none;
        cursor: pointer;
    }

    .nav .nav--content .nav-icon .icon-bar {
        width: 1px;
        height: 2rem;
        background: var(--mk-c-blue-1);
        transition: 0.3s ease-in-out;
    }

    .nav .nav--content .nav-icon .icon-bar:nth-child(2) {
        height: 1.5rem;
    } 

    .nav .nav--content .nav-icon .close-bar:nth-child(1) {
        transform: translateX(8px) rotate(-45deg);
    }

    .nav .nav--content .nav-icon .close-bar:nth-child(2) {
        display: none;
    }

    .nav .nav--content .nav-icon .close-bar:nth-child(2) {
        transform: translateX(-8px) rotate(45deg);
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
        /* .nav {
            margin-bottom: 1.5rem;
        } */

        .nav .nav--content {
            width: var(--width-tablet);
        }

        .nav .nav-items {
            display: flex;
        }

        .nav .nav--content .nav-icon {
            display: none;
        }
    }

    @media screen and (min-width: 1024px) {
        .nav .nav--content {
            width: var(--width-tablet-lg);
        }
    }
  
    @media screen and (min-width: 1200px) {
        .nav .nav--content {
            width: var(--width-desktop);
        }
    }
</style>