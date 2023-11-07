<template>
    <!-- Free Trial -->
    <section class="pt-16">
        <!-- background -->
        <div  class="w-full bg-no-repeat bg-cover relative h-96" style="background-image: url('./img/section3.png');">
            <div v-for="freetrial in freetrials" :key="freetrial._id" class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 z-10 text-white text-center">
                <!-- title -->
                <h1 class="md:text-5xl text-xl mb-5 font-bold leading-relaxed">{{ freetrial.title }}</h1>
                <!-- desc -->
                <p class="md:text-xl text-base mb-5 font-light">{{ freetrial.description }}</p>
                <!-- button -->
                <div class="flex flex-row md:justify-center">
                    <button class="c-button-text-black">
                        <DIV class="c-text-center">
                            Read more
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
                            </svg>
                        </DIV>
                    </button>
                    <button class="c-buttonoutline-text-white">
                        <div class="c-text-center">
                            Contact Us
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
                            </svg>
                        </div>
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            freetrials:[
                {
                    _id: 1,
                    picture: '/img/section3.png',
                    title: 'Join Us by Creating Account or Start a Free Trial',
                    description: 'Install our top-rated dropshipping app to your e-commerce site and get access to US Suppliers, AliExpress vendors, and the best dropshipping and custom products.'
                }
            ]
            
        }
    },
}
</script>