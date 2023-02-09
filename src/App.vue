<template>
	<div>
    <h1>
      <button @click="show">click</button>
    </h1>
	</div>
</template>

<script>
	export default {
    data() {
	    return {
		    num1: 1,
		    num2: 2,
	}
},
  methods: {
	  show: function() {
		  alert(this.num1+this.num2);
	}
}
}
</script>

<style> 
  p{
    color:red;
  }
</style>

