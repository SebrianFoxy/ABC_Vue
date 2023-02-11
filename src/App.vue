<template>
	<div>
  <ul v-for="product in products" :key="product.id">
		{{ product.name }}
	</ul>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        products: [
			{
				id: 1,
				name: 'product1',
			},
			{
				id: 2,
				name: 'product2',
			},
			{
				id: 3,
				name: 'product3',
			},
		]
      }
    },
    methods: {
      
    },
    computed:{
      
    }
  }
</script>

<style> 
  p{
    color:red;
  }
</style>

