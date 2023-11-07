<template>
  <!-- header -->
    <header>
        <!-- container -->
        <div class="c-container">
            <nav class="flex justify-between items-center py-4">
                <!-- logo -->
                <div class="w-2 md:w-20 z-20">
                  <h1 class="text-3xl font-semibold mb-2 text-white">DSP.ONE</h1>
                </div>
                <!-- links -->
                <ul id="menu" class="invisible fixed top-0 left-0 pr-7 w-96 h-screen flex flex-col justify-center items-center bg-gray-900 bg-opacity-90 space-x-4 md:bg-transparent md:h-auto md:flex-row md:justify-between md:static md:visible">
                    <li class="m-12 md:m-0"><a href="#" class="c-link">Home</a></li>
                    <li class="m-12 md:m-0"><a href="#" class="c-link">Features</a></li>
                    <li class="m-12 md:m-0"><a href="#" class="c-link">Course</a></li>
                    <li class="m-12 md:m-0"><a href="#" class="c-link">Blogs</a></li>
                    <li class="m-12 md:m-0"><a href="#" class="c-link">Contact</a></li>
                </ul>
                <!-- button -->
                <button class="c-search">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
                      </svg>                      
                </button>
                <button class="c-trial">
                    <div class="c-text-center">
                        Start Free Trial
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 pl-2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3" />
                        </svg>   
                    </div>                  
                </button>
                <!-- menu button -->
                <div id="menu-button" class="z-20 mr-5 md:hidden cursor-pointer">
                  <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-menu"><line x1="3" y1="12" x2="21" y2="12"></line><line x1="3" y1="6" x2="21" y2="6"></line><line x1="3" y1="18" x2="21" y2="18"></line></svg>
                </div>
            </nav>
        </div>
    </header>
</template>

<script>
export default {

}
</script>
