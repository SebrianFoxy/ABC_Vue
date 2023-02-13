<template>
	<div>
    <input type='text' v-model='textInput' @keyup.enter='addtext'>
    <p>{{ textOutput }}</p>
  </div>
</template>

<script>
  export default{
    data(){
      return{
        textInput: '',
        textOutput: '',
      }
    },
    methods: {
      addtext: function(){
        this.textOutput = this.textInput;
        this.textInput = '';
      }
	  }
}
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

