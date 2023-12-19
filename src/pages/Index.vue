<template>
  <div>
    <h1>Todoリスト</h1>
    <todo-form @handleParentAddTodo="handleParentAddTodo" />
  </div>
</template>

<script>
import TodoForm from '@/components/TodoForm';

export default {
  name: 'Todo',
  components: {
    TodoForm,
  },
  data() {
    return {
      todos: [],
    };
  },
  methods: {
    handleParentAddTodo(value) {
      if (value) {
        this.todos.push({ text: value });
      }
    },
  },
};
</script>

<style scoped>
</style>
