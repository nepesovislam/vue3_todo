<template>
    <div>
        <TodoForm />
        <TodoTabs />
        <TodoItems />
    </div>
</template>

<script setup lang="ts">
import TodoTabs from './partials/TodoTabs.vue';
import TodoForm from './partials/TodoForm.vue';
import TodoItems from './partials/TodoItems.vue'
</script>