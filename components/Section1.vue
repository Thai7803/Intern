<template>
    <!-- section1 -->
    <section class="pt-16">
        <!-- container -->
        <div v-for="section1 in section1s" :key="section1._id" class="flex flex-row justify-evenly items-center py-10">
            <!-- img -->
            <div class="text-center mb-10 flex space-x-1 order-2 w-60 md:space-x-10 md:w-auto">
                <div class="flex-col md:w-60">
                    <img :src="section1.picture1" alt="study1">
                </div>
                <div class="flex-col mt-32 md:w-60 md:mt-40">
                    <img :src="section1.picture2" alt="study2">
                </div>
            </div>
            <!-- text -->
            <div class="text-left order-1 w-44 pl-2 md:w-auto">
                <!-- title -->
                <h2 class="c-title-small">{{ section1.title }}</h2>
                <!-- desc -->
                <p class="c-desc mb-5">{{ section1.description }}</p>
                <!-- button -->
                <button class="c-button-text-black">
                    <div class="c-text-center">
                        Read more
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
                        </svg>
                    </div>
                </button>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            section1s:[
                {
                    _id: 1,
                    picture1: '/img/section1 (1).png',
                    picture2: '/img/section1 (2).png',
                    title: 'eLearning providing the best opportunities to the students around the glob.',
                    description: 'Install our top-rated dropshipping app to your e-commerce site and get access to US Suppliers, AliExpress vendors, and the best dropshipping and custom products. Start selling the right products to the customer base that you know best. We connect you to inventory, so you can focus on creating a catalog of profitable products for your online store.'
                }
            ]
            
        }
    },
}
</script>