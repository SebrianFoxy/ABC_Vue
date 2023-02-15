<template>
	<UserForm @add="add" />
</template>

<script>
import User from './components/User.vue'

export default{
  components: { User },
  methods: {
    add(name, surn) {
      let id = this.users.length + 1;
      
      this.users.push({
        id,
        name,
        surn
      });
    }
  },
  
}
  
</script>




<style> 
p.done{
  text-decoration: line-through;
}
</style>

