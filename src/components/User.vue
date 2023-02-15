<template>
<div>
    <h2>Дочерний компонент</h2>
    <button @click="handle">btn</button>
</div>
</template>

<script>
export default {
    emits:['show'],
    methods: {
	    handle() {
		    this.$emit('show', 'xxx', 'yyy');
	    }
    }
}
</script>


<style>
    
</style>