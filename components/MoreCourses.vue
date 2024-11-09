<template>
    <div class="max-w-3xl mx-auto p-6 pl-0 pt-2 bg-white">
      <h2 class="text-xl font-bold mb-4">
        More Courses by <span class="text-purple-700">Jeff Hendrickson</span>
      </h2>
      <img
          src="https://via.placeholder.com/150"
          alt="Course Thumbnail"
          class="w-56 h-28 object-cover mr-4 mb-2"
        />
      <div class="flex mb-12 w-56">
        <div>
          <h3 class="font-bold mb-1">ChatGPT: Content to Monetize Your Knowledge ...</h3>
          <p class="text-gray-500 text-sm mb-1">Jeff Hendrickson</p>
          <p class="text-gray-500 text-sm mb-1">4 total hours · 43 lectures · Beginner</p>
          <p class="text-gray-900 font-bold">$39.99</p>
        </div>
      </div>
      <hr class="my-4" />
      <button class="w-full border border-gray-900 py-2 text-center text-gray-700 font-bold hover:bg-gray-200">
        Report abuse
      </button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'MoreCourses',
  };
  </script>
  
  <style scoped>
  /* No additional styles needed with Tailwind */
  </style>