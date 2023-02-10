<template>
	<div>
    <h1>
	    <p v-if = "age < 18">Подросток</p>
      <p v-else-if = "age >= 18 && age <= 25">Молодой человек</p>
      <p v-else-if = "age >= 26">Мужчина</p>
      <p v-else>Error</p>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        age: 21,
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

