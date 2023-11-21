<template>
    <!-- Our Courses -->
    <section class="pt-16 bg-gray-800">
        <div>
            <div class="text-center text-white">
                <!-- tag -->
                <h5 class="c-text-orange text-2xl">Our Courses</h5>
                <!-- title -->
                <h1 class=" text-xl text-black font-bold leading-relaxed text-white mb-5 text-center md:text-5xl">Our Best Courses Offered and Teach <br> By Best of The Instructors</h1>
                <!-- desc -->
                <p class="text-lg mb-5 font-light md:text-xl">Install our top-rated dropshipping app to your e-commerce site and get access to US Suppliers, AliExpress vendors, and the best.</p>
            </div>
            <!-- cards -->
            <div class="swiper-container">
              <div class="swiper-wrapper">

              </div>
            </div>
            <div class="grid grid-cols-2 gap-2 px-1 pb-28 md:px-36 md:grid-cols-4 md:gap-4">
                <div v-for="ourcourse in ourcourses" :key="ourcourse._id" class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden w-40 md:w-auto">
                    <img class="h-auto md:w-full" src="../assets/img/course image.png" alt="Card image">
                    <div class="p-4">
                      <h2 class="md:text-xl text-xs font-semibold text-gray-800">{{ ourcourse.title }} <span class="c-text-orange md:pl-7 text-xs md:text-sm">{{ ourcourse.tag }}</span></h2>
                      <p class="text-gray-600 text-xs mt-5 md:text-base">{{ ourcourse.description }} </p>
                      <div class="mt-4 text-sm md:text-base">
                        <b class="c-text-orange text-base md:text-3xl">{{ ourcourse.price }}</b> AED
                      </div>
                      <button class="c-button-view">
                        <div class="c-text-center md:pl-7">
                            View Course 
                        </div>             
                    </button>
                    </div>
                </div>
                <!-- <div class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden w-40 md:w-auto">
                  <img class="h-auto md:w-full" src="../assets/img/course image.png" alt="Card image">
                  <div class="p-4">
                    <h2 class="md:text-xl text-xs font-semibold text-gray-800">Intro to UI/UX <span class="c-text-orange md:pl-7 text-xs md:text-sm">Beginner Level</span></h2>
                    <p class="text-gray-600 text-xs mt-5 md:text-base">Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ... </p>
                    <div class="mt-4 text-sm md:text-base">
                      <b class="c-text-orange text-base md:text-3xl">16.58</b> AED
                    </div>
                    <button class="c-button-view">
                      <div class="c-text-center md:pl-7">
                          View Course 
                      </div>             
                  </button>
                  </div>
              </div>
              <div class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden w-28 md:w-auto hidden md:block">
                <img class="h-auto md:w-full" src="../assets/img/course image.png" alt="Card image">
                <div class="p-4">
                  <h2 class="md:text-xl text-xs font-semibold text-gray-800">Intro to UI/UX <span class="c-text-orange md:pl-7 text-xs md:text-sm">Beginner Level</span></h2>
                  <p class="text-gray-600 text-xs mt-5 md:text-base">Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ... </p>
                  <div class="mt-4 text-sm md:text-base">
                    <b class="c-text-orange text-base md:text-3xl">16.58</b> AED
                  </div>
                  <button class="c-button-view">
                    <div class="c-text-center md:pl-7">
                        View Course 
                    </div>             
                </button>
                </div>
            </div>
            <div class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden w-28 md:w-auto hidden md:block">
              <img class="h-auto md:w-full" src="../assets/img/course image.png" alt="Card image">
              <div class="p-4">
                <h2 class="md:text-xl text-xs font-semibold text-gray-800">Intro to UI/UX <span class="c-text-orange md:pl-7 text-xs md:text-sm">Beginner Level</span></h2>
                <p class="text-gray-600 text-xs mt-5 md:text-base">Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ... </p>
                <div class="mt-4 text-sm md:text-base">
                  <b class="c-text-orange text-base md:text-3xl">16.58</b> AED
                </div>
                <button class="c-button-view">
                  <div class="c-text-center md:pl-7">
                      View Course 
                  </div>             
              </button>
              </div>
            </div> -->
          </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            ourcourses:[
                {
                    _id: 1,
                    picture: '/img/course image.png',
                    title: 'Intro to UI/UX',
                    tag: 'Beginner Level',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...',
                    price: '16.58'
                },
                {
                    _id: 2,
                    picture: '/img/course image.png',
                    title: 'Intro to UI/UX',
                    tag: 'Beginner Level',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...',
                    price: '16.58'
                },
                {
                    _id: 3,
                    picture: '/img/course image.png',
                    title: 'Intro to UI/UX',
                    tag: 'Beginner Level',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...',
                    price: '16.58'
                },
                {
                    _id: 4,
                    picture: '/img/course image.png',
                    title: 'Intro to UI/UX',
                    tag: 'Beginner Level',
                    description: 'Java is a class-based object-oriented simple programming language. Though we can not consider it to be fully ...',
                    price: '16.58'
                }
                
            ]
            
        }
    },
}
</script>