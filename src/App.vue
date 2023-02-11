<template>
	<div>
	  <textarea v-model="text"></textarea>
    <button @click='calc'>click!</button>
    <ul>
      <li v-for="word in words" :key="word">
        {{ word }}
      </li>
    </ul>
  </div>
</template>

<script>
  export default{
    data(){
      return{
        text: '',
        words: [],
      }
    },
    methods: {
      calc: function() {
		    this.words = this.text.split(' ')
	  }
    },
    computed:{
      
    }
  }
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

