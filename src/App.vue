<template>
	<div>
    <button @click="calc" v-bind:disabled="isDisabled">{{isDisabled ? "disable" : "enable"}}</button>
  </div>
</template>

<script>
  export default{
    data(){
      return{
        isDisabled: false,
      }
    },
    methods: {
      calc: function() {
		    this.isDisabled = !this.isDisabled
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

