<template>
    <!-- Meet our team -->
    <section class="pt-16">
        <div>
            <div>
                <div class="text-center">
                    <!-- tag -->
                    <h5 class="c-text-orange text-2xl">MEET OUR TEAM</h5>
                    <!-- title -->
                    <h1 class="c-title-big mb-5 text-center">Expert Teacher</h1>
                </div>
                <!-- cards -->
                <div class="grid grid-cols-3 gap-4 mr-0 md:px-36">
                    <div v-for="team in teams" :key="team._id" class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden w-28 md:w-auto">
                        <img class="w-full h-auto" :src="team.picture" alt="Card image">
                        <div class="p-4">
                          <h2 class="text-lg font-semibold text-gray-800 md:text-xl">{{ team.name}}</h2>
                          <p class="text-gray-600 mt-2">{{ team.job }}</p>
                          <div class="mt-4">
                            <a href="#" class="flex flex-row">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-facebook mr-2"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path></svg>
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-instagram mr-3"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail mr-2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
                            </a>
                          </div>
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
            teams:[
                {
                    _id: 1,
                    picture: '/img/Robert C. Simmons.png',
                    name: 'Robert C. Simmons',
                    job: 'Business Consultant'
                },
                {
                    _id: 2,
                    picture: '/img/Devon Miles.png',
                    name: 'Devon Miles',
                    job: 'Business Consultant'
                },
                {
                    _id: 3,
                    picture: '/img/Tony Danza.png',
                    name: 'Tony Danza',
                    job: 'Business Consultant'
                },
                {
                    _id: 4,
                    picture: '/img/Robert C. Simmons (2).png',
                    name: 'Robert C. Simmons',
                    job: 'Business Consultant'
                },
                {
                    _id: 5,
                    picture: '/img/Devon Miles (2).png',
                    name: 'Devon Miles',
                    job: 'Business Consultant'
                },
                {
                    _id: 6,
                    picture: '/img/Tony Danza (2).png',
                    name: 'Tony Danza',
                    job: 'Business Consultant'
                },
            ]
            
        }
    },
}
</script>