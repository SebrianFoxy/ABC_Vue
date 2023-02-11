<template>
	<div>
    <p :class="{active: isValid, error: isDisabled}">text</p>
    <button @click="setDone">{{ styles.done ? "show" : "hide"}}</button>
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

