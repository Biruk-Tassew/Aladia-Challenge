<template>
    <div class="p-6 pl-0 relative max-w-3xl mx-auto mt-10 mb-10">
      <section class="mb-6">
        <h2 class="text-xl font-bold mb-2">Requirements</h2>
        <ul class="list-disc ml-5">
          <li>There are no prerequisites for this introductory course.</li>
        </ul>
      </section>
      
      <section class="mb-6 relative">
        <h2 class="text-xl font-bold mb-2">Description</h2>
        <div :class="{'max-h-72 overflow-hidden': !showMore}" class="transition-all">
          <p class="mb-2">
            UX and Design Thinking are hot practices in the business world and this course will show you how Design Thinking can help you create the best user experience for your customers.
          </p>
          <p class="mb-2">
            By learning the most important aspects of a user-centric approach, you’ll begin to understand why designing for specific user needs is critical to user adoption, and how to plan for the best possible outcome, whether you're improving an existing application or creating a new one from the ground up.
          </p>
          <p class="mb-2">
            And, you’ll discover just why UX and UI are not the same thing - a misconception that continues to permeate the business world.
          </p>
          <p class="mb-2">
            If you’re in the position of using enterprise software to create applications for end-users, then you want to start with this course to get a solid understanding of what needs to be done for high success rates and user adoption.
          </p>
          <p class="mb-2">
            New module on AI in UX! I've added this new module at the end of March 2024. Whether you've started using AI or not, this new module will show you some of the best ways to incorporate it into your UX practice. And if you're just starting out, having an understanding and skillset in AI is essential so this course brings it all together nicely for you.
          </p>
        </div>
        <div v-if="!showMore" class="absolute bottom-0 left-0 right-0 h-20 bg-gradient-to-t from-white via-white/70 to-transparent"></div>
      </section>
      
      <section v-if="showMore" class="mb-6">
        <h2 class="text-xl font-bold mb-2">Who this course is for:</h2>
        <ul class="list-disc ml-5">
          <li>Anyone involved in applications design and development in business</li>
          <li>Anyone who's looking to be innovative for growth and advancement</li>
          <li>Anyone who works in IT and is responsible for building applications for groups of users</li>
          <li>UX designers and managers who want to understand how AI is changing everything we do</li>
        </ul>
      </section>
      
      <button @click="toggleShowMore" class="text-blue-500 hover:underline flex items-center">
        {{ showMore ? 'Show less' : 'Show more' }}
        <iconify-icon :icon="showMore ? 'mdi:chevron-up' : 'mdi:chevron-down'" class="ml-1"></iconify-icon>
      </button>
    </div>
  </template>
  
  <script>
  import { Icon } from '@iconify/vue';
  
  export default {
    components: {
      IconifyIcon: Icon,
    },
    data() {
      return {
        showMore: false,
      };
    },
    methods: {
      toggleShowMore() {
        this.showMore = !this.showMore;
      },
    },
  };
  </script>
  
  <style scoped>
  </style>