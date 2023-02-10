<template>
	<div>
    <h1>
	    <p v-if="isAdmin">+++</p>
      <p v-else>---</p>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        isAdmin: false,
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

