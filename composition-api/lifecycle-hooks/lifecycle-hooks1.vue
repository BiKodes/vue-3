<template>
    
</template>

<script>
import {onMounted, onUpdated, onUnmounted } from 'vue';

const MyComponent = {
    setup() {
        onMounted(() => {
            console.log('mounted')
        }),

        onUpdated(() => {
            console.log('updated')
        }),

        onUnmounted(() => {
            console.log('unmounted!')
        }),
    }
}

export default {
    
}
</script>