<template>
	<div>
    <h1>
	    <p>Количество продукта: {{amount}} | Цена {{cost}}$</p>
      <p>Всего будет стоить: {{amount*cost}}$</p>
      <button @click="change">click</button>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        cost: 15,
        amount: 10,
      }
    },
    methods: {
      change: function(){
        let newcost = prompt("Введите новую цену");
        this.cost = newcost
      }
    },
    computed:{
      full: function(){
        return this.cost + ' ' + this.amount
      }
    }
  }
</script>

<style> 
  p{
    color:red;
  }
</style>

