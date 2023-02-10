<template>
	<div>
    <template v-for="elem in arr">
		  <p> {{ elem }} </p>
		  <hr>
	  </template>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        arr: [0, 1, 2, 3],
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

