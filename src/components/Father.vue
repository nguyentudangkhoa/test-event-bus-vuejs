<template>
    <div>
        <h1>Test eventBus</h1>
        <Child />
    </div>
</template>

<script>
import Child from './Child'

export default {
    name: 'Father',
    components: {
        Child
    }
}
</script>