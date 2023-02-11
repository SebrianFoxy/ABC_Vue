<template>
	<div>
	  	<input type="checkbox" v-model="checked">
	    <p>{{ checked ? 'yes' : 'no' }}</p>
      <p v-if='checked == true'> Yes yes yes </p>
  </div>
</template>

<script>
  export default{
    data(){
      return{
        checked: 'true',
      }
    },
    methods: {
      calc: function() {
		    this.words = this.text.split(' ')
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

