<template>
	<div>
    <h1>
	    <div v-show="isAuth">
		    <p>+++</p>
		    <p>+++</p>
		    <p>+++</p>
	    </div>
      <button @click="but">
        {{isAuth ? 'hide' : 'show'}}
      </button>
    </h1>
	</div>
</template>

<script>
  export default{
    data(){
      return{
        isAuth: true,
      }
    },
    methods: {
      but: function(){
        this.isAuth = !this.isAuth
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

