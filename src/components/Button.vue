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
        width: 9rem;
        padding: 0.8rem 0;
        border: none;
        border-radius: 5px;
        color: var(--mk-c-text-dark);
        font-size: 0.9rem;
        font-family: 'Lato', sans-serif;
    }
</style>
