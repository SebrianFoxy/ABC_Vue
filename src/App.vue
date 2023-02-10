<template>
	<div>
    <h1>
      <button @click="show">click</button>
      <button @click="cape">Click!!!!!!!!</button>
    </h1>
	</div>
</template>

<script>
	export default {
    data() {
	    return {
		    text: "",
	}
},
  methods: {
	show: function() {
		let text = this.cape(this.text);
	},
	cape: function(str) {
		let day = prompt('Введите число от 1 до 7');
    if (day == 1) {
    alert('Понедельник');
    } 
    else if (day == 2) {
    alert('Вторнк');
    } 
    else if (day == 3) {
    alert('Среда');
    } 
    else if (day == 4) {
    alert('Четверг');
    } 
    else if (day == 5) {
    alert('Пятница');
    } 
    else if (day == 6) {
    alert('Суббота');
    } 
    else if (day == 7) {
    alert('Воскресенье');
    }
    else{
      alert('Ошибка!')
    }
	}
}
}
</script>

<style> 
  p{
    color:red;
  }
</style>

