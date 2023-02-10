<template>
	<div>
    <h1>
	    <button @click="show">btn1</button>
	    <button @click="cape">btn2</button>
    </h1>
	</div>
</template>

<script>
	export default {
    data() {
	    return {
        
	}
},
  methods: {
	show: function() {
		let number = prompt('Введите число');
    alert(number*number)
	},
	cape: function() {
		let number = prompt('Введите число');
    alert(number*number*number)
  }
  }
}
</script>

<style> 
  p{
    color:red;
  }
</style>

