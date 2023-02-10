<template>
	<div>
    <h1>
	    <p v-if="day === 1">Понедельник</p>
      <p v-if="day === 2">Вторник</p>
      <p v-if="day === 3">Среда</p>
      <p v-if="day === 4">Четверг</p>
      <p v-if="day === 5">Пятница</p>
      <p v-if="day === 6">Суббота</p>
      <p v-if="day === 7">Воскресенье</p>
      <p v-else>Число должно быть от 1 до 7</p>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        day: 1,
      }
    },
    methods: {
      
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

