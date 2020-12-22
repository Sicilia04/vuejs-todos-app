<template>
  <div id="app">
    <todos v-model="todos"></todos>
<!--    <todos v-model="todos"></todos>-->
<!--    <todos></todos>-->
<!--    <todos></todos>-->
<!--    <button @click="addTodo">Ajouter une tache</button>-->
  </div>
</template>

<script>
import Todos from './components/Todos.vue'

export default {
  data () {
    return {
      todos: [{
        name: "Demo",
        completed: true
      }]
    }
  },
  name: 'App',
  components: {
    Todos
  },
  methods: {
    addTodo () {
      this.todos.push({
          name: "Jean",
          completed: false
        }
      )
    }
  }
}
</script>
