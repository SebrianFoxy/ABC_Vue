<template>
	<div>
    <h1>
	    <p v-if="hidden1">Первый абзац</p>
      <p v-if="hidden2">Второй абзац</p>
      <p v-if="hidden3">Третий абзац</p>
      <button @click="reversing1">{{hidden1 ? 'hide': 'show'}}</button>
      <button @click="reversing2">{{hidden2 ? 'hide': 'show'}}</button>
      <button @click="reversing3">{{hidden3 ? 'hide': 'show'}}</button>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        hidden1: true,
        hidden2: true,
        hidden3: true,
      }
    },
    methods: {
      reversing1: function(){
        this.hidden1 = !this.hidden1;
      },
      reversing2: function(){
        this.hidden2 = !this.hidden2;
      },
      reversing3: function(){
        this.hidden3 = !this.hidden3;
      }
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

