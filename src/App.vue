<template>
	<div>
		<h1>
      {{ num*num }}
    </h1>
    <h1>
      {{ num1+num2+num3 }}
    </h1>
	</div>
</template>

<script>
	export default {
	data() {
		return {
		  num: 5,
      num1: 1,
		  num2: 2,
		  num3: 3,
		}
	}
}
</script>

<style> 
  p{
    color:red;
  }
</style>

