<template>
	<input v-model="newName">
	<input v-model="newSurn">
	
	<button @click="save">
		save
	</button>
</template>

<script>
export default{
    data() {
        return {
            newName: '',
            newSurn: '',
        }
    },
    methods: {
        save() {
            this.$emit('add', this.newName, this.newSurn);
        }
    },

}
</script>



<style>
    
</style>