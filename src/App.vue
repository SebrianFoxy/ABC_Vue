<template>
	<div>
    <h1>
	    <p><a href="/" onclick="return false">Нажми здесь</a></p>
      <button @click="clicks">click!</button>
      <p>Kol-vo clicks: {{click}}</p>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        click: 0,
      }
    },
    methods: {
      clicks: function(){
        if (this.click == 0){
          return this.click++;
        }
        else{
          alert('Кликнуть можно только 1 раз')
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

