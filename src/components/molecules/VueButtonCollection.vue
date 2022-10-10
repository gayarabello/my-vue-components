<script setup>
import VueButton from "@/components/atoms/VueButton.vue";

const props = defineProps({
    buttons: {
        type: Array,
        required: true
    }
})
</script>

<template>
    <div >
        <VueButton v-for="(button, index) in props.buttons" :key="index" class="mr-8" :options="button"/>  
    </div>
</template>
