<template>
	<div>
    <ul>
		<li v-for="(item, index) in items" :key="index">
			{{ item }}
      <button @click="removeItem(index)">remove</button>
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
      },
      removeItem: function(index) {
		    this.items.splice(index, 1);
	  }
	  }
}
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

