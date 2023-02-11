<template>
	<div>
    <p :class="styles">text</p>
    <button @click="setDone">{{ styles.done ? "show" : "hide"}}</button>
	</div>
</template>

<script>
  export default{
    data(){
      return{
      styles: {
			  done: false,
		},
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

