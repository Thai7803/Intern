<template>
    <!-- section2 -->
    <section class="pt-16">
        <!-- container -->
        <div v-for="section2 in section2s" :key="section2._id" class="flex flex-row justify-evenly items-center py-10">
            <!-- img -->
            <div class="text-center mb-10 w-96 md:w-auto">
                <img :src="section2.picture" alt="study3">
            </div>
            <!-- text -->
            <div class="text-left">
                <!-- title -->
                <h2 class="c-title-small">{{ section2.tile }}</h2>
                <!-- desc -->
                <p class="c-desc mb-5">{{ section2.description }}</p>
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
            section2s:[
                {
                    _id: 1,
                    picture: '/img/section2.png',
                    title: 'We are always working to provide you best of the features in all aspects.',
                    description: 'Install our top-rated dropshipping app to your e-commerce site and get access to US Suppliers, AliExpress vendors, and the best dropshipping and custom products. Start selling the right products to the customer base that you know best. We connect you to inventory, so you can focus on creating a catalog of profitable products for your online store.'
                }
            ]
            
        }
    },
}
</script>