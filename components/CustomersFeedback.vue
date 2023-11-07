<template>
    <!-- Customer's Feedback -->
    <section class="pt-16">
        <div>
            <div>
                <div class="text-center">
                    <!-- tag -->
                    <h5 class="c-text-orange text-2xl">Customer's Feedback</h5>
                    <!-- title -->
                    <h1 class="c-title-big mb-5 text-center">What do customers say about us?</h1>
                </div>
                <!-- container -->
                <div v-for="customer in customers" :key="customer._id" class="flex flex-row justify-evenly items-center pt-10">
                    <!-- img -->
                    <div>
                      <div class="text-center h-52 pb-32 pr-5 md:h-auto md:pr-0 md:pb-0">
                        <img :src="customer.picture" alt="Customer">
                      </div>
                      <p class="c-desc md:hidden">
                        {{ customer.description }}
                      </p>
                    </div>
                    <!-- text -->
                    <div class="text-left">
                        <!-- title -->
                        <h2 class="text-xl text-black font-bold max-w-md leading-relaxed py-1 md:text-4xl">{{ customer.name }}</h2>
                        <!-- tag -->
                        <h5 class="c-text-orange text-base pb-2 md:pb-5 md:text-2xl">{{ customer.job }}</h5>
                        <!-- desc -->
                        <div class="c-desc mb-1 md:mb-5">
                            {{ customer.description }} 
                            <br>
                            <p class="c-desc hidden md:block">
                              {{ customer.description }} 
                            </p>
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
            customers:[
                {
                    _id: 1,
                    picture: '/img/Customer.png',
                    name: 'Lynn Tanner',
                    job: 'Company Name / CEO',
                    description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Blandit id fringilla turpis tempor enim. Vel tristique suspendisse eget sodales egestas. Donec duis lacus, odio velit eu eget ac tortor. Ac sit ultricies hendrerit pellentesque arcu fames sit lectus. Scelerisque id bibendum velit cras.'
                }
            ]
            
        }
    },
}
</script>