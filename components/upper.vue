<template>
    <div class="bg-black text-white md:p-8 lg:p-10">
        <div class="max-w-3xl mx-auto">
            <span class="font-bold text-blue-400 whitespace-nowrap">
                Design
                <span class="inline-flex mx-1 text-blue-200 mb-10">
                    <Icon icon="mdi:chevron-right" />
                </span>
                User Experience Design
                <span class="inline-flex mx-1 text-blue-200">
                    <Icon icon="mdi:chevron-right" />
                </span>
                User Experience (UX) Design
            </span>
            <!-- Course Title -->
            <h1 class="text-2xl md:text-3xl font-bold mb-4">
                UX & Design Thinking Quick Start - Now with AI Module!
            </h1>
            <!-- Course Subtitle -->
            <p class="text-lg md:text-xl mb-6">
                Why This Should Be The Start of Every Application Design Project
            </p>
            <!-- Rating and Student Count -->
            <div class="flex items-center text-yellow-400 mb-4">
                <span class="text-xl font-semibold">4.5</span>
                <star-rating :rating="4.5" :increment="0.5" :read-only="true"></star-rating>
                <a href="#" class="ml-2 text-blue-400">(<span class="underline">5,328 ratings</span>)</a>
                <span class="ml-2 text-gray-300">12,628 students</span>
            </div>
            <!-- Creator and Last Updated -->
            <div class="text-gray-300 text-sm mb-6">
                Created by <a href="#" class="text-blue-400 underline">Jeff Hendrickson</a>
            </div>
            <!-- Bottom Section for Language and Last Updated -->
            <div class="flex items-center text-gray-300 text-sm space-x-4">
                <span class="flex items-center">
                    <Icon icon="mdi:new-releases" class="mr-1 text-white" /> Last updated 3/2024
                </span>
                <span class="flex items-center">
                    <Icon icon="mdi:web" class="mr-1" /> English
                </span>
                <span class="flex items-center">
                    <Icon icon="f7:captions-bubble-fill" style="color: white" /> English [Auto], Dutch [Auto], <a
                        href="#" class="underline">4 more</a>
                </span>
            </div>
        </div>
    </div>
</template>


<script setup>
import { Icon } from '@iconify/vue';
</script>