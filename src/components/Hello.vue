<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <br/>
    <ul>
        <li v-for="user in users">
            {{user.firstName}} {{user.lastName}}: {{user.email}} [{{user.age}}]
        </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Hi, this is a test to show all capabilities of Vue JS.',
      users: [
        {
          firstName: 'Alex',
          lastName: 'Montiel',
          email: 'amontiel@gmail.com',
          age: 23
        },
        {
          firstName: 'Dany',
          lastName: 'Alvez',
          email: 'amontiel@gmail.com',
          age: 23
        },
        {
          firstName: 'Natasha',
          lastName: 'Smith',
          email: 'amontiel@gmail.com',
          age: 23
        },
        {
          firstName: 'Nancy',
          lastName: 'Almeida',
          email: 'amontiel@gmail.com',
          age: 23
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
