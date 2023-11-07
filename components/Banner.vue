<template>
    <!-- Banner -->
    <section class="">
        <!-- container -->
        <div v-for="banner in banners" :key="banner._id" class="flex flex-row justify-evenly items-center py-10">
            <!-- img home -->
            <div class="text-center mb-10 order-2 w-96 pb-64 md:pb-0">
                <img :src="banner.picture" alt="Home">
            </div>
            <div class="text-left order-1 w-44 pl-2 md:w-auto">
                <!-- title -->
                <h1 class="c-title-big py-5 ">{{ banner.titlefirst }} <b class="c-text-orange">expertise</b>, <br>{{ banner.titlesecond }}</h1>
                <!-- desc -->
                <p class="c-desc">{{ banner.description }}</p>
                <!-- button -->
                <div class="pt-10 flex flex-row">
                    <button class="c-button-text-white mb-5">
                        <div class="c-text-center">
                            Register
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
                            </svg>  
                        </div>             
                    </button>
                    <button class="c-buttonoutline-text-orange mb-5">
                        <div class="c-text-center">
                            Login
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
                            </svg>
                        </div>                 
                    </button>
                </div>
                <!-- Course -->
                <div class="relative inline-block text-left pt-3 md:pt-10">
                    <select class="c-select-nemu">
                    <option>Select Course</option>
                    <option>Option 1</option>
                    <option>Option 2</option>
                    <option>Option 3</option>
                    </select>
                    <div class="c-point-down">
                        <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M10.293 14.293a1 1 0 0 1-1.414 0l-3-3a1 1 0 0 1 1.414-1.414L10 12.586l2.293-2.293a1 1 0 0 1 1.414 1.414l-3 3z"/></svg>
                    </div>  
                </div>     
                <div class="relative inline-block text-left pt-3 md:pt-10">
                    <select class="c-select-nemu">
                    <option>Select Instructor</option>
                    <option>Option 1</option>
                    <option>Option 2</option>
                    <option>Option 3</option>
                    </select>
                    <div class="c-point-down">
                        <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M10.293 14.293a1 1 0 0 1-1.414 0l-3-3a1 1 0 0 1 1.414-1.414L10 12.586l2.293-2.293a1 1 0 0 1 1.414 1.414l-3 3z"/></svg>
                    </div>  
                </div>           
                <button class="c-button-text-white mt-5">
                    <div class="c-text-center">
                        Search
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
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
            banners:[
                {
                    _id: 1,
                    picture: '/img/home.png',
                    titlefirst: 'You bring the ',
                    titlesecond: '  we\'ll make it unforgettable.',
                    description: 'Using highly personalised activities, videos and animations you can energise your students and motivate them to achieve their learning goals as they progress through a journey.'
                }
            ]
            
        }
    },
}
</script>