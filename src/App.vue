<template>
	<div>
    <select v-model="selected">
		<option v-for="option in options">{{ option }}</option>
	</select>
	
	<p>{{ selected }}</p>
  </div>
</template>

<script>
  export default{
    data(){
      return{
        selected: 'Понедельник',
		    options: ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье'],
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

