<template>
    <footer class=" bg-[#2d2f31] text-white py-8 mt-10">
        <div>
            <div class="flex justify-between items-center pb-4 max-w-7xl mx-auto">
                <p class="text-lg font-bold">
                    Top companies choose <a href="#" class="text-blue-400 hover:underline">Udemy Business</a> to build
                    in-demand career skills.
                </p>
                <div class="flex space-x-4">
                    <img src="/logos/nasdaq-dark-logo.svg" alt="Nasdaq" class="h-12 w-auto" />
                    <img src="/logos/volkswagen-dark-logo.svg" alt="Volkswagen" class="h-12 w-auto" />
                    <img src="/logos/box-dark-logo.svg" alt="Box" class="h-12 w-auto" />
                    <img src="/logos/netapp-dark-logo.svg" alt="NetApp" class="h-12 w-auto" />
                    <img src="/logos/eventbrite-dark-logo.svg" alt="Eventbrite" class="h-12 w-auto" />
                </div>
            </div>
            <div class="flex justify-between items-center border-b border-gray-700 pb-4"></div>
            <div class="flex justify-between max-w-7xl mx-auto">
                <!-- Grid with links -->
                <div class="grid grid-cols-3 gap-8 py-8 max-w-3xl">
                    <div class="flex flex-col space-y-2">
                        <a href="#" class="hover:underline">Udemy Business</a>
                        <a href="#" class="hover:underline">Teach on Udemy</a>
                        <a href="#" class="hover:underline">Get the app</a>
                        <a href="#" class="hover:underline">About us</a>
                        <a href="#" class="hover:underline">Contact us</a>
                    </div>
                    <div class="flex flex-col space-y-2">
                        <a href="#" class="hover:underline">Careers</a>
                        <a href="#" class="hover:underline">Blog</a>
                        <a href="#" class="hover:underline">Help and Support</a>
                        <a href="#" class="hover:underline">Affiliate</a>
                        <a href="#" class="hover:underline">Investors</a>
                    </div>
                    <div class="flex flex-col space-y-2">
                        <a href="#" class="hover:underline">Terms</a>
                        <a href="#" class="hover:underline">Privacy policy</a>
                        <a href="#" class="hover:underline">Cookie settings</a>
                        <a href="#" class="hover:underline">Sitemap</a>
                        <a href="#" class="hover:underline">Accessibility statement</a>
                    </div>
                </div>

                <!-- Button -->
                <button
                    class="flex items-center space-x-2 h-10 border border-gray-700 px-3 py-3 hover:bg-gray-800 mt-6">
                    <Icon icon="mdi:web" class="h-5 w-5" />
                    <span class="pr-8">English</span>
                </button>
            </div>
            <div class="flex justify-between items-center pt-4  max-w-7xl mx-auto mb-12">
                <img src="/logos/udemy-inverted-logo.svg" alt="Udemy" class="h-8 w-auto" />
                <p class="text-sm text-white">&copy; 2024 Udemy, Inc.</p>
            </div>
        </div>
    </footer>
</template>

<script>
import { Icon } from '@iconify/vue';

export default {
    name: 'FooterComponent',
    components: {
        Icon
    }
}
</script>

<style scoped>
/* Additional styles if necessary */
</style>