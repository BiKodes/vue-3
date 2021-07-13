<template>
    
</template>

<script>
export default {
    setup() {
        const internalInstance = getCurrentInstance()    // works

        const id = useComponentId()      // works

        const handleClick = () => {
            getCurrentInstance() // doesn't work
            useComponentId()     // doesn't work

        internalInstance //works

        }

    onMounted(() => {
        getCurrentInstance() //works
    })

    return () => 
        h(
            'button',
            {
                onClick: handleClick
            },
            `uid: ${id}`
        )
        
    }
    // also works if called on a composable
    function useComponentId() {
        return getCurrentInstance().uid
    }
    
}
</script>