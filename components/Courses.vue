<template>
    <div class="flex flex-col justify-between max-w-3xl mx-auto mt-10 w-full">
        <h3 class="text-2xl font-bold">Course content</h3>
        <div class="flex justify-between items-center mt-7 mb-2">
            <p class="">9 sections • 25 lectures • 3h 1m total length</p>
            <a href="#" class="text-purple-600 font-bold hover:underline">Expand all sections</a>
        </div>
        <div class="border-2 flex-1 border-gray-100 bg-gray-100">
            <!-- Wrap the v-for in a parent element -->
            <div v-for="accordian in accordianLists" :key="accordian.text">
                <CourseContents :course="accordian" />
            </div>
        </div>
    </div>
</template>

<script setup>
import CourseContents from "./CourseContent.vue";

const accordianLists = [
    {
        status: "Completed",
        icon: "✅",
        text: "Introduction to Cloud Computing",
        time: "2024-11-08",
    },
    {
        status: "In Progress",
        icon: "⏳",
        text: "Introduction to Web Development with HTML, CSS, JavaScript",
        time: "2024-11-05",
    },
    {
        status: "Not Started",
        icon: "❌",
        text: "Getting Started with Git and GitHub",
        time: "2024-11-07",
    },
    {
        status: "Completed",
        icon: "✅",
        text: "Developing Front-End Apps with React",
        time: "2024-11-01",
    },

    {
        status: "Completed",
        icon: "✅",
        text: "Introduction to Containers w/ Docker, Kubernetes & OpenShift",
        time: "2024-10-28",
    },
    {
        status: "In Progress",
        icon: "⏳",
        text: "Application Development using Microservices and Serverless",
        time: "2024-10-27",
    },
    {
        status: "Not Started",
        icon: "❌",
        text: "Full Stack Cloud Development Capstone Project",
        time: "2024-10-25",
    },
    {
        status: "In Progress",
        icon: "⏳",
        text: "Full Stack Software Developer Assessment",
        time: "2024-10-24",
    },
];
</script>