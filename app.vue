<template>
  <div>
    <Navbar />
    <Banner />
    <TrustCompanies />
    <Section1 />
    <Section2 />
    <FreeTrial />
    <Features />
    <OurCourses />
    <Meetourteam />
    <CustomersFeedback />
    <BlogPosts />
    <Footer />
    <!-- <CardShow /> -->
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Banner from '@/components/Banner.vue'
import TrustCompanies from '@/components/TrustCompanies.vue'
import Section1 from '@/components/Section1.vue'
import Section2 from '@/components/Section2.vue'
import FreeTrial from '@/components/FreeTrial.vue'
import Features from '@/components/Features.vue'
import OurCourses from '@/components/OurCourses.vue'
import Meetourteam from '@/components/Meetourteam.vue'
import CustomersFeedback from '@/components/CustomersFeedback.vue'
import BlogPosts from '@/components/BlogPosts.vue'
import Footer from '@/components/Footer.vue'
//import CardShow from '@/components/CardShow.vue'

export default { 
  components: {
    Navbar,
    Banner,
    TrustCompanies,
    Section1,
    Section2,
    FreeTrial,
    Features,
    OurCourses,
    Meetourteam,
    CustomersFeedback,
    BlogPosts,
    Footer
    //CardShow,
  }

}
</script>
  

<style>

</style>