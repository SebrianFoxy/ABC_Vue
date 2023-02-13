<template>
	<div>
    <ul>
		<li v-for="(item, index) in items" :key="index">
			{{ item }}
		</li>
	</ul>
  	<input v-model="newitem">
	  <button @click="addItem">add</button>
  </div>
</template>

<script>
  export default{
    data(){
      return{
        newitem: '',
        items: ['a', 'b', 'c'],
      }
    },
    methods: {
      addItem: function(){
        this.items.push(this.newitem)
      }
	  }
}
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

