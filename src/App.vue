<template>
	<div>
    <p>Где живешь?</p>
  <select v-model="selected">
		<option>В Рассия</option>
		<option>Где-то</option>
		<option>На планете Земля</option>
	</select>
    <p>{{ selected }}</p>
  </div>
</template>

<script>
  export default{
    data(){
      return{
        selected: 'value1',
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

