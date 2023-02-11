<template>
	<div>
	  <input v-model="num1">
    <input v-model="num2">
	  <button v-on:click="calc">work</button>
    <p>{{ res }}</p>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        num1: 0,
        num2: 0,
		    res: 0,
      }
    },
    methods: {
      calc: function() {
		    this.res = parseInt(this.num1) + parseInt(this.num2)
	  }
    },
    computed:{
      
    }
  }
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

