<template>
    <div class="border border-gray-300 p-6 max-w-3xl mx-auto mt-10">
      <h2 class="text-xl font-bold mb-6">Frequently Bought Together</h2>
      <div class="relative">
        <CourseCard
          image="https://via.placeholder.com/150"
          title="UX & Design Thinking Quick Start - Now with AI Module!"
          instructor="Jeff Hendrickson"
          rating="4.5"
          reviews="5,325"
          price="39.99"
        />
        <div class="absolute left-20 top-24 z-10 flex">
          <div class="rounded-full bg-white border border-gray-300 p-2">
            <iconify-icon icon="mdi:plus" class="text-gray-800" height="24" width="24" />
          </div>
        </div>
        <CourseCard
          image="https://via.placeholder.com/150"
          title="User Experience Design Fundamentals"
          instructor="Joe Natoli"
          rating="4.5"
          reviews="16,638"
          price="64.99"
        />
        <div class="absolute left-20 top-56 z-10 flex">
          <div class="rounded-full bg-white border border-gray-300 p-2">
            <iconify-icon icon="mdi:plus" class="text-gray-800" height="24" width="24" />
          </div>
        </div>
        <CourseCard
          image="https://via.placeholder.com/150"
          title="UX & Web Design Master Course: Strategy, Design, Development"
          instructor="Joe Natoli"
          rating="4.6"
          reviews="15,393"
          price="64.99"
        />
      </div>
      <div class="flex justify-between items-center mt-6">
        <div class="text-lg">
          Total: <span class="text-black  font-bold">$169.97</span>
        </div>
        <button class="bg-purple-500 text-white py-2 px-4  font-bold hover:bg-purple-600">
          Add all to cart
        </button>
      </div>
    </div>
  </template>
  
  <script>
  import CourseCard from './CourseCard.vue';
  import { Icon } from '@iconify/vue';
  
  export default {
    components: {
      CourseCard,
      IconifyIcon: Icon,
    },
  };
  </script>
  