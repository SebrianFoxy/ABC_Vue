<template>
	<div>
    <p :style="{color: 'green', 'font-weight': 'bold', background: 'yellow'}">
		  text
	  </p>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        isValid: true,
		    isDisabled: true,
      }
    },
    methods: {
      setDone: function(){
        this.styles.done = !this.styles.done
      }
    },
    computed:{
      
    }
  }
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

