<template>
	<div>
    <h1>
	    {{text}}
      <button @click="change">btn1</button>
      <button @click="change1">btn2</button>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        text:"xxx",
      }
    },
    methods: {
      change: function(){
        this.text="yyy"
      },
      change1: function(){
        this.text="zzz"
      }
    }
  }
</script>

<style> 
  p{
    color:red;
  }
</style>

