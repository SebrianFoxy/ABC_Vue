<template>
	<div>
    <ul>
		<template v-for="elem in items">
			<li v-if="elem > 0">
				{{ elem }}
			</li>
		</template>
	</ul>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        items: [1, -2, 3, -4, 5],
      }
    },
    methods: {
      
    },
    computed:{
      
    }
  }
</script>

<style> 
  p{
    color:red;
  }
</style>

