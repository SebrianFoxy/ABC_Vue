<template>
	<div>
    <li v-for="(elem, key, index) in obj">
		  {{ key }} -
		  {{ elem }} -
      {{ index + 1 }}
	  </li>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        obj: {
          user1: '100$',
	        user2: '200$',
	        user3: '300$',
        },
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

