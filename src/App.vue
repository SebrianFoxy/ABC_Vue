<template>
  <div>
    <User
      v-for="user in users"
      :id="user.id"
      :name="user.name"
      :surn="user.surn"
      @remove="remove(user.id)"
      :key="user.id"
    />
  </div>
</template>

<script>
import User from './components/User.vue'

export default {
  components: { User },
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'name1',
          surn: 'surn1'
        },
        {
          id: 2,
          name: 'name2',
          surn: 'surn2'
        },
        {
          id: 3,
          name: 'name3',
          surn: 'surn3'
        },
      ],
    }
  },
  methods: {
    remove(id) {
      this.users = this.users.filter(user => user.id !== id)
    }
  }
}
</script>




<style> 
p.done{
  text-decoration: line-through;
}
</style>

