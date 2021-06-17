<template>
    <div>
        <img alt="Vue logo" src="../assets/logo.png">
        <Button />
    </div>
</template>

<script>
import Button from './Button';
import EventBus from '../EventBus';

export default {
    name: 'Child',
    components: {
        Button
    },
    created() {
        EventBus.$on('setEventBus', this.handler)
    },
    methods: {
        handler(data) {
            alert('Hello: ' + data);
        }
    }
}
</script>