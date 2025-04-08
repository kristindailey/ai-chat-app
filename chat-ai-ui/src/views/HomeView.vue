<script setup lang="ts">
    import { ref } from "vue";
    import robotImage from "../assets/robot.png";

    const name = ref("");
</script>

<template>
    <div class="h-screen flex items-center justify-center bg-gray-900 text-white">
        <div class="p-8 bg-gray-800 rounded-lg shadow-lg w-full max-w-md">
            <img :src="robotImage" alt="Robot image" class="mx-auto w-24 h-24 mb-4">
            <h1 class="text-2xl font-semibold mb-4 text-center">
                Welcome to Chat AI
            </h1>

            <input type="text" class="w-full p-2 mb-2 bg-gray-700 text-white rounded-lg focus:outline-none" placeholder="Name" v-model="name">
        </div>
    </div>
</template>