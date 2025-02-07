<template>
    <div class="mt-10">
        <div class="grid grid-cols-1 sm:hidden">
            <select aria-label="Select a tab" class="col-start-1 row-start-1 w-full appearance-none rounded-md bg-white/5 py-2 pl-3 pr-8 text-base text-white outline outline-1 -outline-offset-1 outline-white/10 focus:outline focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-500">
                <option v-for="tab in tabs" :key="tab.name" :selected="tab.current">{{ tab.name }}</option>
            </select>
            <PhArrowDown class="pointer-events-none col-start-1 row-start-1 mr-2 size-5 self-center justify-self-end fill-gray-400" aria-hidden="true" />
        </div>
        <div class="hidden sm:block">
            <nav class="flex py-4">
                <ul role="list" class="flex min-w-full flex-none justify-center gap-x-8 px-2 text-sm/6 font-semibold text-white">
                    <li v-for="tab in tabs" :key="tab.name">
                        <a :href="tab.href" :class="tab.current ? 'text-indigo-400 bg-gray-200 rounded-md px-3 py-2' : ''">{{ tab.name }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>
  
<script setup>
import { PhArrowDown } from '@phosphor-icons/vue';
  
const tabs = [
    { name: 'All', href: '#', current: true },
    { name: 'Active', href: '#', current: false },
    { name: 'Compeleted', href: '#', current: false },
]
</script>