<script setup lang="ts">
import useCounterStore from "../stores/counter";

const counterStore = useCounterStore();

</script>

<template>
    <div class="p-8 grid  text-center">
        <h1 class="text-2xl font-bold mb-4">Home Page</h1> 
        <p class="text-lg">This is the home page content.</p>
        <p class="text-lg">Counter: <span class="font-bold">{{ counterStore.count }}</span></p>
        <div class="mt-4">
            <button type="button" @click="counterStore.increment" class="text-white bg-blue-700 hover:bg-blue-800  focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Counter++</button>
        </div>
        
    </div>
</template>