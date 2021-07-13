<template>
    
</template>

<script>
// used to sync the type of the injected value between the provider and the consumer:

import { InjectionKey, provide, inject} from 'vue';

 const key: InjectionKey<string> = Symbol()
   
    // providing non-string value will result in error
   provide(key, 'foo')

    // type of foo: string | undefined
   const foo = inject(key)
   
export default {
  
}
</script>