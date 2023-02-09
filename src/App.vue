<template>
	<div>
		<h1>
      {{ arr[0] }}
    </h1>
    <h1>
      {{ arr[1] }}
    </h1>
    <h1>
      {{ arr[2] }}
    </h1>
    <h1>
      {{ arr1[0]+arr1[1]+arr1[2] }}
    </h1>
	</div>
</template>

<script>
	export default {
	data() {
		return {
		  arr: ['x', 'y', 'z'],
      arr1: [1, 2, 3],
		}
	}
}
</script>

<style> 
  p{
    color:red;
  }
</style>

