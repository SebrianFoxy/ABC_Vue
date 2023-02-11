<template>
	<div>
    <input name="radio" type="radio" v-model="choice" value="v1">
	  <input name="radio" type="radio" v-model="choice" value="v2">
	  <input name="radio" type="radio" v-model="choice" value="v3">
    you choosed: {{ choice }}    
  </div>
</template>

<script>
  export default{
    data(){
      return{
        choice: '',
      }
    },
    methods: {
      calc: function() {
		    this.text = this.arr.split(' ')
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

