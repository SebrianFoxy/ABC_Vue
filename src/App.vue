<template>
	<div>
		<p>{{ name }}</p>
    <p>{{ surn }}</p>
	</div>
</template>

<script>
	export default {
	data() {
		return {
			name: 'john',
		  surn: 'smit',
		}
	}
}
</script>

<style> 
  p{
    color:red;
  }
</style>