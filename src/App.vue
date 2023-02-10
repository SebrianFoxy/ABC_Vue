<template>
	<div>
    <h1>
	    <p v-if="visible1">{{click}}</p>
      <p v-if="visible2">{{click}}</p>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        click: 1500,
        visible1: true,
        visible2: false,
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

