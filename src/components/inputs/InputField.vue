<template>
    <div class="flex flex-col">
        <label class="font-medium text-[14px] leading-[16.59px] lg:text-base mb-[10px]" v-if="label">{{ label }}</label>
        <slot />
    </div>
</template>
<script setup>
    import { defineProps } from "vue"

    defineProps({
        label: String,
        default: null,
    })
</script>