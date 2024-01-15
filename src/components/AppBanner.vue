<script setup>
    import BlurBg from '@/assets/bg_blur.png';
</script>
<template>
    <div :style="{ backgroundImage: `url(${BlurBg})`}" class="min-h-[325px] bg-cover bg-center bg-no-repeat flex flex-col justify-center px-[17px] lg:px-[100px] white-text">
        <div class="container mx-auto">
            <div class="flex flex-row flex-nowrap gap-x-2 lg:gap-x-3 mb-10 lg:mb-6 items-center">
                <img src="@/assets/Home.png" class="h-[18px] w-[18px] lg:w-[24px] lg:h-[24px]">
                <span class="text-[14px] leading-[16.59px]  lg:text-lg">/</span>
                <span class="text-[14px] leading-[16.59px]  lg:text-lg">Contact</span>
            </div>
            <h1 class="text-[24px] lg:text-[40px] mb-4 font-medium">Contact</h1>
            <p class="text-[14px] leading-[16.59px] lg:text-base lg:leading-[18.96px]">Heb je nog vragen of wil je gewoon even kletsen over voetbal? Neem contact op via een van de onderstaande opties en we staan je graag te woord. Ook ben je tijdens kantooruren van harte welkom bij ons op kantoor in Maarssen!</p>
        </div>
    </div>
</template>