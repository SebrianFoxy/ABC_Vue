<template>
	<div>
    <input v-model="message">
	  <p>{{ message*message }}</p>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        message: 'Hello',
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

