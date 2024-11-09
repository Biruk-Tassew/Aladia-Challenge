<template>
    <div class="flex max-w-3xl mx-auto">
        <div class="flex-1">
            <div class="">
                <h2 class="text-xl font-semibold">Students also bought</h2>
                <div v-for="(course, index) in courses" :key="index"
                    class="flex items-start space-x-4 p-4 pl-0 border-b-2 border-gray-100">
                    <img :src="course.image" alt="Course image" class="w-24 h-24" />
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold mb-2">{{ course.title }}</h3>
                        <div class="flex gap-2 items-center">
                            <p class="text-sm px-2 bg-lime-200">
                                {{ course.tag }}
                            </p>
                            <p class="text-sm font-bold text-green-600">
                                {{ course.hours }} total hours
                            </p>
                            <p class="text-sm text-gray-500">Updated {{ course.updated }}</p>
                        </div>
                    </div>

                    <p class="flex items-center text-yellow-500 space-x-1">
                        <Icon icon="ic:round-star" class="w-5 h-5" />
                        <span>{{ course.rating }}</span>
                    </p>
                    <p class="text-sm text-gray-500">
                        <Icon icon="mdi:account-multiple" class="w-4 h-4 inline-block mr-1" />
                        {{ course.students }} students
                    </p>
                    <div class="text-right flex gap-2">
                        <p class="text-xl font-semibold">${{ course.price }}</p>
                        <button class="text-gray-500 hover:text-gray-700">
                            <Icon icon="mdi:heart-outline" class="w-6 h-6" />
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { Icon } from "@iconify/vue"; // Correct import for Iconify

const courses = [
    {
        image:
            "https://plus.unsplash.com/premium_photo-1726191984484-a37113aa3cc4?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxmZWF0dXJlZC1waG90b3MtZmVlZHwyfHx8ZW58MHx8fHx8",
        title: "Entrepreneurship: How To Start A Business From An Idea",
        rating: 4.6,
        students: 41620,
        updated: "9/2024",
        hours: "12.5",
        price: 69.99,
        tag: "Bestseller",
    },
    {
        image:
            "https://plus.unsplash.com/premium_photo-1726191984484-a37113aa3cc4?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxmZWF0dXJlZC1waG90b3MtZmVlZHwyfHx8ZW58MHx8fHx8",
        title: "The Business Startup Guide to Become an Entrepreneur",
        rating: 4.8,
        students: 2767,
        updated: "11/2024",
        hours: "25",
        price: 69.99,
        tag: "Bestseller",
    },
    {
        image:
            "https://plus.unsplash.com/premium_photo-1726191984484-a37113aa3cc4?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxmZWF0dXJlZC1waG90b3MtZmVlZHwyfHx8ZW58MHx8fHx8",
        title: "The Complete Business Plan Course (Includes 50 Templates)",
        rating: 4.7,
        students: 175233,
        updated: "3/2024",
        hours: "9",
        price: 69.99,
        tag: "Bestseller",
    },
    {
        image:
            "https://plus.unsplash.com/premium_photo-1726191984484-a37113aa3cc4?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxmZWF0dXJlZC1waG90b3MtZmVlZHwyfHx8ZW58MHx8fHx8",
        title: "How to come up with killer business ideas: complete workshop",
        rating: 4.5,
        students: 75878,
        updated: "11/2024",
        hours: "7",
        price: 64.99,
        tag: "Bestseller",
    },
];
</script>

<style scoped>
/* Optional: Add custom styles if needed */
</style>