<template>
    <div class="max-w-3xl mx-auto p-6 pl-0 bg-white rounded-lg">
        <h2 class="text-2xl font-bold mb-4">Instructor</h2>
        <InstructorDetails :instructor="instructor" />
        <RetractableParagraph :text="instructor.bio" />
    </div>
</template>

<script>
import InstructorDetails from './InstructorDetails.vue';
import RetractableParagraph from './RetractableParagraph.vue';

export default {
    components: {
        InstructorDetails,
        RetractableParagraph,
    },
    data() {
        return {
            instructor: {
                name: 'Jeff Hendrickson',
                tagline: 'Good Design Sustains Us, Great Design Moves Us',
                image: 'https://via.placeholder.com/150',
                rating: 4.5,
                reviews: 5325,
                students: 12631,
                courses: 2,
                bio: `Starting off long ago in the clothing industry in NYC, I've traveled the world as a researcher, designer, strategist, and product developer.  I have a passion for teaching because I love to see that look in the eyes of a student when the lightbulb turns on and they blossom in the world.  I'm a storyteller, I'm an artist, I'm a lover of life.
            In my tenure in the tech industry I've briefed the Asst Secretary of Defense on knowledge management projects, I've consulted with GM, The Chicago Board of Trade and others, and I've reviewed Business Intelligence and Analytics projects for many Fortune 500 companies.
            I am currently the UX Research Manager for a top five international  paper and packaging company, where I coach younger UXers, evangelize up the enterprise, and set standards of excellence for UX practices.  I use the exact same methods I teach in this course to help every company I work with see and understand where they have problems, and then to design solutions to those problems that save them millions of dollars a month or year in wasted costs.`,
            }
        };
    }
};
</script>

<style scoped>
/* No additional styles needed with Tailwind */
</style>