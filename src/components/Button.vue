<template>
    <div>
        <button @click="setEventBus">Get Event Bus</button>
    </div>
</template>

<script>
import EventBus from '../EventBus';

export default {
    name: "Button",
    data() {
        return {
            alert: 'Hello Khoa'
        }
    },
    methods: {
        setEventBus() {
            EventBus.$emit('setEventBus', this.alert);
        }
    }
}
</script>