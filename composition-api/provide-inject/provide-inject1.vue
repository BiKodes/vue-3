<script>
// Typing:

interface InjectionKey<T> extends Symbol {}

function provide<T>(key: InjectionKey<T> | string, value: T): void

// without default value
function inject<T>(key: InjectionKey<T> | string): T | undefined

// with default value
function inject<T>(key: InjectionKey<T> | string, defaultValue: T): T



// with factory

function inject<T>(
    key: InjectionKey<T> | string,
    defaultValue: () => T,
    treatDefaultAsFactory: true
    ): T


export default {
    
}
</script>