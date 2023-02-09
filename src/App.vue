<template>
	<div>
		<h1>
      <button @mouseover="show">text</button>
    </h1>

    <h1>
      <button @click="show">text</button>
    </h1>
	</div>
</template>

<script>
	export default {
	data() {
		
	},
	methods: {
		show: function(){
      alert('09.02.2022');
    }
	}
}
</script>

<style> 
  p{
    color:red;
  }
</style>

