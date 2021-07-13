<template>
    
</template>
// Arguments:
<script>
// checking the absence of an optional prop  give it a Symbol as its default value::

const isAbsent = Symbol()

export default {
    props: {
        foo: { default: isAbsent }
    },

    setup(props) {
        if (props.foo === isAbsent) {

        }

        
    }
     // Typing:
    interface Data {
        [key: String]: unknown

    }   
    interface SetupContext {
        attrs:  Data
        slots: Slots
        emit: (event: string, ...args: unknown[] => void)
    }
    function setup(props: Data, context: SetupContext): Data
        
    
    }
   


}

</script>

