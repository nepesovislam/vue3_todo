<template>
    <div>
        <h2 class="text-center text-3xl font-semibold tracking-tight text-white sm:text-5xl">{{props.title}}</h2>
    </div>
</template>

<script setup lang="ts">
const props = defineProps({
    title: {
        type: String,
        required: true,
    },
});
</script>
  