<template>
	<div>
    <p v-for="num in 30">
		{{ num }}
	</p>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        users: [
			{
				name: 'name1',
				surn: 'surn1',
			},
			{
				name: 'name2',
				surn: 'surn2',
			},
			{
				name: 'name3',
				surn: 'surn3',
			},
		]
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

