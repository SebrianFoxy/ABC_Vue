<template>
	<User :arg="[1, 2, 3]" />
</template>

<script>
  import User from './components/User.vue'
  export default{
    components:{
      User
    },
    data(){
      return{
        
      }
	}
}
</script>

<style> 
p.done{
  text-decoration: line-through;
}
</style>

