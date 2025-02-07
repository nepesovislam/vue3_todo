<template>
    <div class="my-24 mx-auto max-w-2xl sm:px-6 lg:px-8">
        <PageHeading :title="title" />
        <Todo />
    </div>
</template>

<script setup lang="ts">
import PageHeading from '@/components/common/PageHeading.vue';
import Todo from '@/components/todo/Todo.vue';

const title = 'ToDo';
</script>