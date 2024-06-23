<template>
    <div id="Profile" class="flex flex-col justify-center items-center">
        <div class="mt-5 flex flex-row justify-center items-center">
            <picture class="mr-3">
                <img src="../../assets/profile.jpg" class="w-32 h-32 md:w-40 md:h-40 lg:w-48 lg:h-48 rounded-full border-4 border-gray-300 shadow-lg">
            </picture>
            <div class="ml-3 flex flex-col justify-center items-center">
                <h1 class="great-vibes-regular font-mono mb-4 text-4xl font-extrabold leading-none tracking-tight text-gray-900 md:text-5xl lg:text-6xl dark:text-white"> Sofronea </h1>
                <h1 class="great-vibes-regular mb-4 text-4xl font-extrabold leading-none tracking-tight text-gray-900 md:text-5xl lg:text-6xl dark:text-white"> Georgian </h1>
            </div>
        </div>
    
        <p class="mt-5 playwrite-nz-regular text-white text-xl md:text-2xl lg:text-3xl"> Welcome !  </p>
        <hr class="mt-5 w-1/2 mx-auto">
        <p class="mt-5 playwrite-nz-regular text-white text-xl md:text-2xl lg:text-3xl"> I'm glad you landed here. </p>
    </div>

    
</template>


<style>
    .great-vibes-regular {
        font-family: "Great Vibes", cursive;
        font-weight: 400;
        font-style: normal;
    }

    .playwrite-nz-regular {
        font-family: "Playwrite NZ", cursive;
        font-optical-sizing: auto;
        font-weight: 300;
        font-style: normal;
    }
</style>