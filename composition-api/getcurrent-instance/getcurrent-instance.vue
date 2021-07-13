<template>
    
</template>

<script>
import { getCurrentInstance } from 'vue';

const MyComponent = {
    setup() {
        const internalInstance = getCurrentInstance()

        internalInstance.appContext.config.globalProperties
    }
}
export default {
    
}
</script>