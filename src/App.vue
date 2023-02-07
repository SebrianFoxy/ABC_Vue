<template>
	<div>
		<h1>
      Перейдите по ссылке <a :href="href"> {{ text }}</a>
    </h1>
	</div>
</template>

<script>
	export default {
	data() {
		return {
		  text: 'page',
		  href: 'page.html',
		}
	}
}
</script>

<style> 
  p{
    color:red;
  }
</style>