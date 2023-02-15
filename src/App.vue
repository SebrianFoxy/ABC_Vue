<template>
  <div>
    <h2>Работники:</h2>
    <ul>
      <li v-for="user in users" 
        :name="user.name"
        :surn="user.surn"
        :key="user.id">
        <p>Имя: {{ user.name }}</p>
        <p>Зарплата: {{ user.salary }}</p>
        <p>Возраст: {{ user.age }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'name1',
          salary: 100,
          age: 30,
        },
        {
          id: 2,
          name: 'name2',
          salary: 200,
          age: 40,
        },
        {
          id: 3,
          name: 'name3',
          salary: 300,
          age: 50,
        },
      ],
    }
  },
}
</script>


<style> 
p.done{
  text-decoration: line-through;
}
</style>

