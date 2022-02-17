<script>
    export default {
        name: "Button",
        props: {
            "action": String,
            "background": String,
        }
    }
</script>

<template>
    <button class="cta-btn" :style="{ background: `${background}` }">{{ action }}</button>
</template>

<style scoped>
    .cta-btn {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 13.5rem;
        padding: 1.5rem 0;
        border: none;
        border-radius: 5px;
        color: var(--mk-c-text-dark);
        font-size: 1.2rem;
        font-family: 'Nunito', sans-serif;
    }

    @media screen and (min-width: 640px) {
        .cta-btn {
            width: 12rem;
            padding: 1rem 0;
            font-size: 1rem;
        }
    }
</style>
