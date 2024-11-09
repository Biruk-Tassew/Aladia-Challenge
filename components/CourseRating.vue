<template>
    <div class="max-w-3xl mx-auto p-6 pl-0 bg-white">
        <div class="flex items-center mb-6">
            <iconify-icon icon="mdi:star" class="text-yellow-500 mr-2"></iconify-icon>
            <span class="text-xl font-bold">4.5 course rating · 5K ratings</span>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 gap-x-10">
            <ReviewCard v-for="(review, index) in reviews" :key="index" :review="review" />
        </div>
        <button class="mt-6 border border-gray-800 px-4 py-2 hover:bg-gray-100 font-bold text-gray-700">
            Show all reviews
        </button>
    </div>
</template>

<script>
import ReviewCard from './ReviewCard.vue';
import { Icon } from '@iconify/vue';
export default {
    components: {
        ReviewCard,
        IconifyIcon: Icon,
    },
    data() {
        return {
            reviews: [
                {
                    initials: 'SB',
                    name: 'Sayandeep - Ext B.',
                    rating: 4,
                    time: 'a month ago',
                    text: 'It was good but lacked any real learning outcomes. More detail would have been great.',
                },
                {
                    initials: 'JH',
                    name: 'Jeffrey H.',
                    rating: 5,
                    time: 'a month ago',
                    text: "No fat, all of it (doesn't make sense...yet) but very straight ahead communication.",
                },
                {
                    initials: 'DM',
                    name: 'Diego Diaz M.',
                    rating: 3,
                    time: 'a month ago',
                    text: 'Buen contenido, mala presentación... principalmente la sección sobre IA, al usar siempre el mismo texto, no alternar imágenes o darle un poco más de dinamismo, se siente pesado y difícil de seguirle el paso.',
                },
                {
                    initials: 'SU',
                    name: 'Surabhi Gupta U.',
                    rating: 4,
                    time: '3 months ago',
                    text: 'Course is really insightful and covered important topics with less theory.AI section could be improved as mostly explanation is repetitive with new & twisted words.',
                },
            ],
        };
    },
};
</script>

<style scoped>
/* No additional styles needed with Tailwind */
</style>