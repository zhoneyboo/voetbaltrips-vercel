<template>
    <InputField :label="label">
        <input type="text" class="px-[16px] py-[9px] lg:px-[16px] lg:py-[12.5px] common-border rounded-md focus:outline-none text-base focus:border-[#006FEB]"  v-bind="$attrs">
    </InputField>
</template>
<script setup>
    import InputField from '@/components/inputs/InputField.vue';
    import { defineProps } from "vue"

    defineProps({
        label: {
            type: String,
            default: null
        },
    })
</script>