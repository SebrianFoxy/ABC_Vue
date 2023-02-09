<template>
	<div>
		<h1>
      {{ obj.x + obj.y + obj.z}}
    </h1>
	</div>
</template>

<script>
	export default {
	data() {
		return {
		  obj: {x: 1, y: 2, z: 3},
		}
	}
}
</script>

<style> 
  p{
    color:red;
  }
</style>

