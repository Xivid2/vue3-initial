<script setup lang="ts">
    import { ref } from "vue";

    let count = ref(0);

    const addToCount = () => {
        count.value += 1;
    };

    const subtractFromCount = () => {
        count.value -= 1;
    };
</script>

<template>
    <main>
        <h4>The current count is...</h4>
        <h1>{{ count }}</h1>
        <button @click="subtractFromCount()">-</button>
        <button @click="addToCount()">+</button>
    </main>
</template>

<style>
    body {
        background-color: aliceblue;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    main {
        text-align: center;
    }
</style>