<template>
    <div>{{ readersNumber }} {{ book.title }}</div>
</template>

<script>
import { ref, reactive } from 'vue';

export default {
   setup() {
       const readersNumber = ref(0)
       const book = reactive({title: 'Vue 3 Tour'})
      
      
      return {
          readersNumber,
          book
      }
   } 
}
</script>