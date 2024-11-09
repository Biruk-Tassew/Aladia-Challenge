<template>
    <div class="grid grid-cols-2 gap-4 border border-gray p-6 max-w-3xl bg-white mt-10 mx-auto">
        <h2 class="text-2xl font-bold mb-4 col-span-2">What you'll learn</h2>
        <div>
            <ul class="space-y-3">
                <li v-for="(item, index) in leftColumnItems" :key="index" class="flex items-start">
                    <Icon icon="material-symbols-light:check" width="32" height="32"
                        class="text-black mr-2 font-bold" />
                    <span>{{ item }}</span>
                </li>
            </ul>
        </div>
        <div class="ml-4">
            <ul class="space-y-3">
                <li v-for="(item, index) in rightColumnItems" :key="index" class="flex items-start">
                    <Icon icon="material-symbols-light:check" width="32" height="32"
                        class="text-black mr-2 font-bold" />
                    <span>{{ item }}</span>
                </li>
            </ul>
        </div>
    </div>
</template>

<script setup>
import { Icon } from '@iconify/vue';
</script>
<script>
export default {
    data() {
        return {
            leftColumnItems: [
                "Understand how UX & Design Thinking form the core of every successful project.",
                "Learn the crucial interviewing skills necessary to ensure you're building the right application for the right people.",
                "Learn how to incorporate AI tools and technology to enhance your UX design work."
            ],
            rightColumnItems: [
                 "Understand the importance of UX & Design Thinking for application design projects.",
                "Learn a new way to break down larger problem sets into chunks that more clearly identify the problems.",
            ]
        };
    }
};
</script>

<style scoped>
/* Tailwind utility classes already handle styling */
</style>