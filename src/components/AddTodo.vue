<template>
  <div>
    <form @submit="addToDo">
      <input
          type="text"
          v-model="title"
          name="title"
          placeholder="Add Todo..."
      >
      <input type="submit" value="Submit" class="btn">
    </form>
  </div>
</template>

<script>
export default {
  name: 'AddTodo',
  data() {
    return {
      title: ''
    }
  },
  methods: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  form {
    display: flex;
  }
  input[type="text"]{
    flex: 10;
    padding: 5px;
  }
  input[type="submitt"]{
    flex: 2;
  }

</style>
