<template>
	<div>
    <h1>
	    <ul v-for="(elem, key) in arr">
		  {{ key }} {{ elem }}
      </ul>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        arr: ['x', 'y', 'z'],
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

