<template>
	<template v-if="!isEdit">
		{{ name }}
		{{ surn }}
		<button @click="edit">
			edit
		</button>
	</template>
	<template v-else>
		<input v-model="newName">
		<input v-model="newSurn">
		<button @click="save">
			save
		</button>
	</template>
</template>

<script>
export default {
    props: {
	id:     Number,
	name:   String,
	surn:   String,
},
    emits: ['change'],
    data() {
        return {
            isEdit: false,
            newName: this.name,
            newSurn: this.surn,
        }
    }, 
    methods: {
	save() {
		this.isEdit = false;
		this.$emit('change', this.id, this.newName, this.newSurn);
	}
},  
};
</script>



<style>
    
</style>