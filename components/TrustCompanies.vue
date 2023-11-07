<template>
    <!-- Trust Companies -->
    <section class="pt-16">
        <div v-for="company in companies" :key="company._id">
            <!-- title -->
            <h2 class="text-1xl text-black font-bold leading-relaxed mr-6 mb-5 text-center md:text-5xl md:mr-0">{{ company.title }}</h2>
            <!-- companies -->
            <div class="flex space-x-5 ml-6 w-10 md:space-x-20 md:pl-20 md:w-auto md:mt-20">
                <img :src="company.pictureGG" alt="Google">
                <img :src="company.pictureNet" alt="Netflix">
                <img :src="company.pictureAir" alt="Airbnb">
                <img :src="company.pictureAma" alt="Amazon">
                <img :src="company.pictureFB" alt="Facebook">
                <img :src="company.pictureGrab" alt="Grab">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            companies: [
                {
                    _id: 1,
                    title: 'Trusted by 5,000+ Companies Worldwide',
                    pictureGG: '/img/google.png',
                    pictureNet: '/img/netflix.png',
                    pictureAir: '/img/airbnb.png',
                    pictureAma: '/img/amazon.png',
                    pictureFB: '/img/facebook.png',
                    pictureGrab: '/img/grab.png',
                }
            ]
        }
    },
}
</script>