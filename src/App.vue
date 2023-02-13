<template>
	<div>
    <ul>
		<li v-for="user in users" :key="user.id">
			{{ user.name }}
      {{ user.surn }}
      <button @click="removeItem(user.id)">remove</button>
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
        users: [
			{
				id: 1,
				name: 'name1',
				surn: 'surn1',
			},
			{
				id: 2,
				name: 'name2',
				surn: 'surn2',
			},
			{
				id: 3,
				name: 'name3',
				surn: 'surn3',
			},
		]
      }
    },
    methods: {
      removeItem: function(id) {
		    this.users = this.users.filter((user) => {
			return user.id !== id;
		})
	  }
	  }
}
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

