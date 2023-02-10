<template>
	<div>
    <h1>
	    <div v-for="elem in items">
		    <p>{{elem}}</p>
	    </div>
      <p>Квадрат чисел</p>
      <div v-for="elem in items">
        <p>{{elem*elem}}</p>
      </div>
      <div v-for="elem in items">
        <ul>{{elem*elem}}</ul>
      </div>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        items: [1, 2, 3, 4, 5],
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

