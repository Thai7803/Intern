<template>
    <!-- Blog Posts -->
    <section class="pt-16">
        <div>
            <div>
                <div class="text-center">
                    <!-- tag -->
                    <h5 class="c-text-orange text-2xl">Blog Posts</h5>
                    <!-- title -->
                    <h1 class="c-title-big mb-5 text-center">Articles will help to to stay up to date <br> with all the knowledge</h1>
                    <!-- desc -->
                    <p class="text-base mb-5 font-light md:text-xl">Install our top-rated dropshipping app to your e-commerce site and get access to US Suppliers, AliExpress vendors, and the best.</p>
                </div>
                <!-- cards -->
                <div class="grid grid-cols-2 gap-2 px-1 md:px-36 pb-28 md:grid-cols-3 md:gap-3">
                    <div v-for="blog in blogs" :key="blog._id" class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden">
                        <img class="w-full h-auto" :src="blog.picture" alt="Card image">
                        <div class="p-4">
                          <h2 class="text-sm font-semibold text-gray-800 md:text-xl">{{blog.title}}</h2>
                          <p class="text-gray-600 mt-5 text-xs md:text-base">{{blog.description}} </p>
                          <button class="c-buttonoutline-text-orange mt-5">
                            <div class="c-text-center">
                                Read Article
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                                    <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
                                </svg>
                            </div>             
                          </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            blogs:[
                {
                    _id: 1,
                    picture: '/img/Rectangle 32.png',
                    title: 'Why Java is best programming language?on',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...'
                },
                {
                    _id: 2,
                    picture: '/img/Rectangle 32 (1).png',
                    title: 'Why Java is best programming language?',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...'
                },
                {
                    _id: 3,
                    picture: '/img/Rectangle 32 (2).png',
                    title: 'Why Java is best programming language?ation',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...'
                },
                {
                    _id: 4,
                    picture: '/img/Rectangle 32 (3).png',
                    title: 'Why Java is best programming language?icing',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...'
                },
                {
                    _id: 5,
                    picture: '/img/Rectangle 32 (4).png',
                    title: 'Why Java is best programming language?faction',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...'
                },
                {
                    _id: 6,
                    picture: '/img/Rectangle 32 (5).png',
                    title: 'Why Java is best programming language?terials',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...'
                }
            ]
            
        }
    },
}
</script>