<template>
    <div class="w-full flex flex-column justify-between lg:block">
        <div class="flex flex-row flex-nowrap items-center gap-x-4 mb-2">
            <div class="w-[34px] lg:w-[32px] h-[24px] lg:h-[32px] flex flex-row items-center justify-center">
                <img :src="icon">
            </div>
            <div class="flex-grow">
                <p class="mb-0 lg:text-base font-medium leading-[18.96px] uppercase text-[#006FEB]">{{ label }}</p>
            </div>
        </div>
        <div class="flex flex-row flex-nowrap items-center gap-x-4">
            <div class="w-[34px] lg:w-[32px] hidden lg:flex flex-row"></div>
            <div class="flex-grow text-base leading-[18.96px] lg:text-[18px] lg:leading-[21.33px]">
                <slot>
                    <p class="mb-0">
                        {{  content }}
                    </p>
                </slot>
            </div>
        </div>
    </div>
</template>
<script setup>
    import { defineProps } from "vue";

    defineProps({
        label: {
            type: String,
            default: null
        },
        content: {
            type: String,
            default: null
        },
        icon: {
            type: String,
            default: null,
        }
    })
</script>