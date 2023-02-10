<template>
	<div>
    <h1>
	    <p v-if="hidden">Первый абзац {{click}}</p>
      <p v-if="!hidden">Второй абзац</p>
      <button @click="reversing">Reverse</button>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        click: 1500,
        hidden: true,
      }
    },
    methods: {
      reversing: function(){
        if (this.hidden == true){
          this.hidden = false;
        }
        else if (this.hidden == false){
          this.hidden = true;
        }
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

