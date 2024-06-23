<template>
    <div id="About" class="mt-7 mb-12 ml-5 mr-5 w-100">
        <h2 class="ml-4 underline playwrite-nz-regular mb-4 text-3xl font-extrabold leading-none tracking-tight text-gray-900 md:text-4xl lg:text-5xl dark:text-white">About me</h2>
        <p class="courier-new mb-4 text-xl leading-none tracking-tight text-gray-900 md:text-2xl dark:text-white">
            I'm a {{ age }} year old student in the capital of Romania, where I came with an adventurous soul and ambitious mind, albeit reluctant sometimes, but in continuous discovery.
        </p>
        <p class="courier-new mb-4 text-xl leading-none tracking-tight text-gray-900 md:text-2xl dark:text-white">
            Everyday I'm happy to see people in a good mood; so do me a favor and put a smile on your face, but don't fake it if you can't. 
        </p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            birthDate: '2003-04-07'
        };
    },
    computed: {
        age() {
            let diff = new Date().getFullYear() - new Date(this.birthDate).getFullYear();
            const todayMonth = new Date().getMonth();
            const birthMonth = new Date(this.birthDate).getMonth();

            if (todayMonth < birthMonth || (todayMonth === birthMonth && new Date().getDate() < new Date(this.birthDate).getDate())) {
                diff--;
            }

            return diff;
        }
    }
}

</script>

<style>
    .courier-new {
        font-family: "Courier New", cursive;
        font-optical-sizing: auto;
        font-weight: 300;
        font-style: normal;
    }
    p {
        text-align:justify; 
        text-justify:auto; 
        text-indent: 50px; 
    }
</style>