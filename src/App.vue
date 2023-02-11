<template>
	<div>
  <p v-for="elem in arr">
		{{ elem }}
	</p>
	<button @click="add">add</button>
  <button @click="del">delete</button>
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

