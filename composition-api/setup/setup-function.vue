<template>
    
</template>

<script>
import { h, ref, reactive } from 'vue';

export default {
    setup() {
        const readersNumber = ref(0)
        const book = reactive({title: 'Vue 3 Ninja'})
    }

    // explicitly exposing ref value here

    return () => h('div', [readersNumber.value, book.title])

}
</script>