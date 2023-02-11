<template>
	<div>
    <p>Hello</p>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        arr: ["a"],
        a:"",
      }
    },
    methods: {
      add: function(){
        this.a = prompt("Введите то, что хотите добавить")
        this.arr.push(this.a)
      },
      del: function(){
        this.arr.pop()
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

