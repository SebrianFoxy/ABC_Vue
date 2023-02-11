<template>
	<div>
    <p>Твои любимые языки:</p>
	  <p>English <input type="checkbox" v-model="arr" value="English"></p>
	  <p>Russian <input type="checkbox" v-model="arr" value="Russian"></p>
	  <p>Japan <input type="checkbox" v-model="arr" value="Japan"></p>
    <ul>
      <li v-for="word in arr">
        {{word}}
      </li>
    </ul>
    
  </div>
</template>

<script>
  export default{
    data(){
      return{
        arr: [],
        text: '',
      }
    },
    methods: {
      calc: function() {
		    this.text = this.arr.split(' ')
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

