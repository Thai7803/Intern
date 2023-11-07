<template>
    <!-- Features -->
    <section class="pt-16">
        <div>
            <div class="text-center">
                <!-- tag -->
                <h5 class="c-text-orange text-2xl">Features</h5>
                <!-- title -->
                <h1 class="c-title-big mb-5 text-center">By Joining eLearning Platform,<br> One Can Avail a Lot Of Benefits.</h1>
                <!-- desc -->
                <p class="text-xs mb-5 font-light md:text-xl">Install our top-rated dropshipping app to your e-commerce site and get access to US Suppliers, AliExpress vendors, and the best.</p>
            </div>
            <!-- cards -->
            <div class="grid grid-cols-3 gap-4 px-1 pb-28 md:px-32">
                <div v-for="feature in features" :key="feature._id" class="col-span-1 bg-white-200 p-4">
                  <!-- tag -->
                  <h1 class="c-text-orange text-lg mb-5 md:text-3xl">{{ feature.number }}</h1>
                  <!-- title -->
                  <div class="font-bold text-sm mb-2 md:text-xl">{{ feature.title }}</div>
                  <!-- desc -->
                  <p class="text-gray-700 text-xs md:text-base">
                      {{ feature.description }} <a href="#"><b class="c-text-orange">Read More</b></a>
                  </p>
                </div>
              </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            features:[
                {
                    _id: 1,
                    number: '01',
                    title: 'Standardization',
                    description: 'When working in a global workplace, it’s often difficult to gauge learners’ training experiences, which are ...'
                },
                {
                    _id: 2,
                    number: '02',
                    title: 'Reduced Costs',
                    description: 'With eLearning, there’s no cost to reproduce materials and, thanks to mobile learning and microlearning, learners can ...'
                },
                {
                    _id: 3,
                    number: '03',
                    title: 'More Customization',
                    description: 'Just like learners aren’t one-size-fits-all, learning is not a one-size-fits-all experience. By using different ...'
                },
                {
                    _id: 4,
                    number: '04',
                    title: 'Affordable Pricing',
                    description: 'With eLearning, there’s no cost to reproduce materials and, thanks to mobile learning and microlearning, learners can ...'
                },
                {
                    _id: 5,
                    number: '05',
                    title: 'Learner Satisfaction',
                    description: 'If you really want students to retain what they learn, you’ll need to aim for high satisfaction rates. Bad ...'
                },
                {
                    _id: 6,
                    number: '06',
                    title: 'Multimedia Materials',
                    description: 'One of the main reasons why custom eLearning is effective is that it’s the perfect delivery method for ...'
                }
            ]
            
        }
    },
}
</script>