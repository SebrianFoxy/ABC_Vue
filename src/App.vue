<template>
  <div>
    <h1>Родительский компонент</h1>
    <User @show="func" />
  </div>
</template>

<script>
import User from './components/User.vue';

export default {
  components: {
    User
  },
  methods: {
	  func(arg1, arg2) {
		  alert(arg1, arg2);
	  }
  },
}
</script>



<style> 
p.done{
  text-decoration: line-through;
}
</style>

