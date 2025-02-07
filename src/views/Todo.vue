<template>
    <div class="px-6 py-8 sm:py-16 lg:px-8">
        <div class="mx-auto max-w-2xl text-center">
            <PageHeading :title="title" />
            <Todo />
        </div>
    </div>
</template>

<script setup lang="ts">
import PageHeading from '@/components/common/PageHeading.vue';
import Todo from '@/components/todo/Todo.vue';

const title = 'ToDo';
</script>